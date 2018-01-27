# Grouping & Selectors {#top}
CSS allows you to be as generic or as specific as you want. In this section we will learn how to apply styles to multiple selectors and work with special selectors. 

This section will help guide you through the following steps:
---- 
 * Set default color for headers
 * Change hover color using pseudo classes
 * Add space between list items
 
----

## Set default color for all header text {#header-colors} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
Setting a style on multiple selectors at once makes CSS succinct. In this section you'll set a default color for all header text.
{% include "./1header-colors.md" %}

## Change hover color of hyperlinks {#link-stylesheet} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
Providing user feedback on clickable elements such as hyperlinks is thoughtful user interaction. You'll set a hover color, style lists, and practice CSS organization.
{% include "./2hover-color.md" %}

## Resize images using relative and absolute sizes {#resize} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
We'll work some more with list styling and add spacing between list elements.
{% include "./3list-item-space.md" %}


## Checkpoint
Your _styles.css_ file should look like this

PICTURE HERE OF PAGE AND REPLACE CODE WITH IMAGE

```css
body {
  background-color: #fefaec;
}

h1, h2, h3, h4, h5, h6 {
        color: #637056;
}

nav {
  background-color: #cb6f10;
}

nav ul {
  list-style-type: none;
}

nav a:hover {
  background-color: #d88731;
}

.hero h1 {
  color: #cb6f10;
}

.hero h2 {
  color: #cb6f10;
}

.hero p {
  color: #cb6f10;
}

.drinks img {
  width: 120px;
  height: 120px;
}

.sidebar {
  background-color: #d9e9ce;
}

.sidebar ul {
  list-style-type: none;
}

.sidebar ul li {
  margin-top: 50px;
}

.sidebar ul li:first-child {
  margin-top: 0;
}

footer {
  background-color: #cb6f10;
}

footer ul {
  list-style-type: none;
}

footer a:hover {
  background-color: #d88731;
}
```


## References and helpful links
[Mozilla Developer Network CSS selector documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors)

[Mozilla Developer Network styling list documentation](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Styling_lists)