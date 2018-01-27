# BONUS
Users expect to interact with webpages using their mobile devices. Building a fully responsive webpage is not an easy undertaking, but media queries and layout systems like CSS Grid help make this faster.

Before starting this assignment, view the completed LadyDev Bar & Grill in Chrome. Resize the browser to decrease the width. Notice regardless of the width the drinks menu and small plates menu display side to side. Let's use a media query to have the small plates menu display after the drinks menu when the width is 700px or less.

{% hint style='tip' %}
##### Hey Slacker!

Remember, we're here to help.
Join the KCWiT #codingandcocktails Slack Channel: [kcwit.slack.com](http://kcwit.slack.com)
{% endhint %}


### Define grid template areas

1. Declare a grid template area for the drinks menu by adding `grid-area: drinks;` to the styles for the `div` with `class="drinks"`. 
1. Declare a grid template area for the Small plates menu sidebar. Name it "sidebar".  
1. Save the file and reload the page in Chrome. 😕
  {% hint style='working' %}
Where did the drinks menu go?  
CSS Grid doesn't know how to lay out the two template areas you defined, so it placed both in the same column. Add `display:none;` to the Small plates sidebar `div` in Chrome Dev Tools to see the drinks menu.
   {% endhint %}
1. Define the layout order of the two grid template areas you declared in the `.grid-container` style by adding 
    ```css
    grid-template-areas:
    "drinks sidebar";
    ```
1. Save the file and reload the page in Chrome to see everything return to normal.
  {% hint style='working' %}
Try changing the order of "drinks" and "sidebar" in the `grid-template-areas` and see what happens in the browser.
  {% endhint %}


### Add media query
1. Create a new style under the styles defined for `.grid-container` targeting a screen media type and a maximum width of 700px. Your style should looks like
  ```css
  @media screen and (max-width: 700px) {

  }
  ```
  {% hint style='tip' %}
You can see the width of your app when using Chrome Dev Tools and looking at the Box Model diagram in the **Styles** tab.
  {% endhint %}
1. Copy the `.grid-container` style and paste it inside the media query. Save your file and reload the page in Chrome. Resize the browser to decrease width. You won't see any changes yet because you have the same styles applied both screen widths.
1. To define 2 rows, split the `grid-areas` to separate entries. Edit the `grid-template-areas` in the media query to
  ```css
    grid-template-areas:
    "drinks" 
    "sidebar";
  ```
1. Save the file, reload in Chrome, and resize the browser. Almost there!
1. We still see a margin to the right side where the Small plates menu used to be. Now that we have one column, fix the `grid-template-columns` in the media query.
  {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
We need 1 column in the media query. Change "grid-template-columns" to "auto;". 
</details>
   {% endhint %}


### References and helpful links
[Mozilla Developer Network Media query documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)
[Mozilla Developer Network Grid template areas documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout/Grid_Template_Areas)
[Grid By Example](https://gridbyexample.com/examples/)


Answer Key (to check in and post a link)
```css
@import url(https://fonts.googleapis.com/css?family=Montserrat|Neuton);

/* Reset */
html, body, div, h1, h2, h3, h4, h5, h6, p, a,
img, li, aside, footer, nav, section {
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: inherit;
}

body {
  background-color: #fefaec;
  font-family: Neuton, "Times New Roman", Times, serif;
}

h1, h2, h3, h4, h5, h6 {
  color: #637056;
  font-family: Montserrat, Arial, Helvetica, sans-serif;

}

nav {
  background-color: #cb6f10;
  border-bottom: 5px solid #f1a250;
  text-align: right;
  font-family: Montserrat, Arial, Helvetica, sans-serif;
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
  color: #ffffff;
  font-weight: bold;
  text-decoration: none;
  font-size: 1.5em;
}

nav a:hover {
  background-color: #d88731;
}

.hero {
  height: 600px;
  background: url("../images/hero.jpg") no-repeat center top;
  background-size: cover;
}

.hero-text {
    padding-top: 125px;
    width: 50%;
    text-align: center;
}

.hero h1 {
  color: #cb6f10;
  font-size: 5em;
}

.hero h2 {
  color: #cb6f10;
  font-size: 1.5em;
  margin-bottom: 20px;
}

.hero p {
  color: #cb6f10;
  font-size: 1.25em;
}

.grid-container {
  display: grid;
  grid-template-columns: 75% auto;
  grid-template-areas:
  "drinks sidebar";
}

@media screen and (max-width: 700px) {
  .grid-container {
    display: grid;
    grid-template-columns: auto;
    grid-template-areas:
    "drinks"
    "sidebar";
  }
}

.drinks {
  grid-area: drinks;
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.drinks h2 {
  font-size: 3em;
  margin: 5px;
}

.drinks .item {
  border-top: 1px dotted #637056;
  padding-top: 10px;
  margin-bottom: 60px;
  display: block;
}

.drinks .head {
  font-size: 2em;
}

.drinks p {
  font-size: 1.3em;
}

.drinks img {
  margin: 0 20px;
  width: 120px;
  height: 120px;
  border-radius: 50%;
  float: left;
}

.sidebar {
background-color: #d9e9ce;
font-size: 1.5em;
grid-area: sidebar;
}

.sidebar h2 {
  font-size: 2em;
  text-align: center;
  margin: 5px 0;
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

footer p {
  color: white;
  text-align: center;
  margin-bottom: 15px;
}

footer ul {
  list-style-type: none;
  display: block;
  margin: 0;
  padding: 0;
  text-align: center;
}

footer li {
  display: inline-block;
}

footer i {
  color: white;
  padding: 2px 10px;
}

footer a:hover {
  background-color: #d88731;
}

```
