# Accessibility
## Semantic HTML Elements

```
<header>
  <!--Header Elements-->
</header>

<nav>
</nav>

```

## ARIA
(Aria)[https://www.w3.org/TR/html-aria/#allowed-aria-roles-states-and-properties]
### ROLE

**complementary**
To help add context to web page information, ARIA provides an HTML attribute called role. The value of an element’s role changes how a screen reader communicates the element

<div id="code-editor" role="complementary">
  ...
</div>


the role="complementary" attribute and value can help a screen reader user understand that the information in the code editor is complementary (or supporting) to the information you are reading right now. It helps users of screen readers identify the relationship between the two sections of the page.

**presentation**
skips over elements and their necessary children. The <ol> and <ul> elements require <li> children. Therefore, adding role="presentation" to an ol tag will cause the screen reader to skip directly to the text between the <li> tags (it will not read the names of the <li> elements).
  
```
<ol role="presentation">
  <li>List Item 1</li>
  <li>List Item 2</li>
</ol>
```

**properties**
property aria-label gives the screen reader additional information to read out loud to the user

```
<img src="#" alt="A painting of the Shenandoah Valley"/>
<p aria-label="Artist">Armand Cabrera, 2010</p>
```

