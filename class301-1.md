## Responsive Web Design
Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.
### Flexible Layouts
Responsive web design is broken down into three main components, including flexible layouts, media queries, and flexible media. The first part, flexible layouts, is the practice of building the layout of a website with a flexible grid,
capable of dynamically resizing to any width. 
Flexible grids are built using relative length units, most commonly percentages or em units. These relative lengths are then used to declare common grid property values such as width, margin, or padding.
### Flexible Grid
The flexible layout approach alone isn’t enough.media queries can be used to help build a better experience.
**html**
`<div class="container">
  <section>...</section>
  <aside>...</aside>
</div>`
**css for fixed grid demo** 
`.container {
  width: 538px;
}
section,
aside {
  margin: 10px;
}
section {
  float: left;
  width: 340px;
}
aside {
  float: right;
  width: 158px;
}
`
**css for flixible grid demo**
`section,
aside {
  margin: 1.858736059%; /*  10px ÷ 538px = .018587361 */
}
section {
  float: left;
  width: 63.197026%;    /* 340px ÷ 538px = .63197026 */   
}
aside {
  float: right;
  width: 29.3680297%;  /* 158px ÷ 538px = .293680297 */
}
`
### Media Queries
There are a couple different ways to use media queries, using the @media rule inside of an existing style sheet, importing a new style sheet using the @import rule, or by linking to a separate style sheet from within the HTML document.
Generally speaking it is recommend to use the @media rule inside of an existing style sheet to avoid any additional HTTP requests.
**html**
`<!-- Separate CSS File -->
<link href="styles.css" rel="stylesheet" media="all and (max-width: 1024px)">
`
**css**
`/* @media Rule */
@media all and (max-width: 1024px) {...}

/* @import Rule */
@import url(styles.css) all and (max-width: 1024px) {...}
`
### Logical Operators in Media Queries
There are three different logical operators available for use within media queries, including and, not, and only.
`@media all and (min-width: 800px) and (max-width: 1024px) {...}`
`@media not screen and (color) {...}`
## All About Floats
What is “Float”?Float is a CSS positioning property. element wrap will allow the elements to flow over the element.
`#sidebar {
  float: right;			
}`
There are four valid values for the float property. Left and Right float elements those directions respectively.
### Clearing the Float
Float’s sister property is clear. An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float.
`#footer {
  clear: both;			
}`
Clear has four valid values as well. Both is most commonly used, which clears floats coming from either direction.
## grid context
**Columns**
`<div class="grid">
  <div class="col-2-3">
     Main Content
  </div>
  <div class="col-1-3">
     Sidebar
  </div>
</div>`
**css**
`[class*='col-'] {
  float: left;
}
.col-2-3 {
  width: 66.66%;
}
.col-1-3 {
  width: 33.33%;
}`
## Gutters
The hardest part about grids is gutters. So far we’ve made our grid flexible by using percentages for widths.
The first step toward this is using box-sizing: border-box;
`*, *:after, *:before {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}`
The second step is applying a fixed padding to the right side of all columns except the last one.
`[class*='col-'] {
  padding-right: 20px;
}
[class*='col-']:last-of-type {
  padding-right: 0;
}`
## SMACSS
**“SMACSS is becoming one of the most useful contributions to front-end discussions in years”**
What is it?
it is more style guide than rigid framework. There is no library within here for you to download or install. There is no git repository for you to clone. 
SMACSS is a way to examine your design process and as a way to fit those rigid frameworks into a flexible thought process. It is an attempt to document a consistent approach to site development when using CSS.
