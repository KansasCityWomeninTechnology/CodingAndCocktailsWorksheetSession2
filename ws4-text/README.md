# Text {#top}
With layout complete, styling text adds the final polish to a website. Using a different font for sections of the web page adds interest and appeal. 

<!-- trick markdown to give me a little space between these two sections of text -->
## 

This section will help guide you through the following steps:
{% include "./checklist.html" %}

## Normalize style for cross browser consistency {#normalize} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
Your users will use different browsers. Help your users have a consistent browsing experience by resetting all styles.
{% include "./1normalize.md" %}

## Select header and body fonts and define fallback fonts  {#select-fonts} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
Different fonts help define areas. But you have to have a backup plan. Let's select fonts for our web page and define fallback fonts as a contingency.
{% include "./2select-fonts.md" %}

## Define font styles {#fonts} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
Beautiful text adds final polish to websites. You will resize and decorate text to polish LadyDev Bar & Grill website.
{% include "./3fonts.md" %}

## Style icon fonts {#icon-fonts} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
Social icons are a must for any website. Let's style them so they match our website's theme.
{% include "./4icon-fonts.md" %}

## Checkpoint
Your _styles.css_ file should look like this

PICTURE HERE OF PAGE AND REPLACE CODE WITH IMAGE

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
}

.drinks {
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


## References and helpful links
[Mozilla Developer Network Font properties documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/font)

[Mozilla Developer Network Text properties documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Text)


