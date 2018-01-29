# Box Model & Layout {#top}
Cluttered web pages overload the brain. Spacing and layout helps draw attention to different parts of the website by making it easier for users to "see". We will continue our work on LadyDev Bar & Grill by applying spacing and layout concepts.

<!-- trick markdown to give me a little space between these two sections of text -->
## 

This section will help guide you through the following steps:
{% include "./checklist.html" %}

## Define section boundaries with borders {#borders} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
Borders help define sections and helps the user by grouping like items together. You will explore different border properties to bring definition to your webpage.
{% include "./1borders.md" %}

## Use the Box Model to add padding and margins  {#padding-margin} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
The Box Model is use to declare spacing. You will apply Box Model concepts to add whitespace to LadyDev Bar & Grill.
Refer to the [CSS Cheat Sheet](../references/css_cheat_sheet.md) to help.
{% include "./2padding-margin.md" %}

## Define a background image to use for the hero image {#hero} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
Most eye-catching websites have a hero image. Let’s learn about background properties and use what we learned about absolute and relative sizing and apply it to the hero image.
{% include "./3hero.md" %}

## Use CSS grid for layout {#grid-layout} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
We want the drink menu and small plates menu as two columns next to each other. We will use CSS Grid to make this easy.
{% include "./4grid-layout.md" %}

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
  border-bottom: 5px solid #f1a250;
}

nav ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

nav li {
  padding: 2px;
  display: inline;
}

nav a {
  padding: 6px 20px;
  display: inline-block;
}

nav a:hover {
  background-color: #d88731;
}

.hero {
  height: 600px;
  background: url("../images/hero.jpg") no-repeat center top;
  background-size: cover;
}

.hero h1 {
  color: #cb6f10;
}

.hero h2 {
  color: #cb6f10;
  margin-bottom: 20px;
}

.hero p {
  color: #cb6f10;
}

.grid-container {
  display: grid;
  grid-template-columns: 75% auto;
}

.drinks {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.drinks .item {
  border-top: 1px dotted #637056;
  padding-top: 10px;
  margin-bottom: 60px;
  display: block;
}

.drinks img {
  width: 120px;
  height: 120px;
  border-radius: 50%;
  margin: 0 20px;
}

.sidebar{
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
  border-top: 5px solid #f1a250;
  height: 75px;
}

footer ul {
  list-style-type: none;
  display: block;
  margin: 0;
  padding: 0;
}

footer li {
  display: inline-block;
}

footer a:hover {
  background-color: #d88731;
}

```


## References and helpful links
[Mozilla Developer Network Box Model documentation](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Box_model)

[Mozilla Developer Network Display documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/display)

[Mozilla Developer Network Background documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/background)

[Mozilla Developer Network Grid Layout documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout/Basic_Concepts_of_Grid_Layout)
