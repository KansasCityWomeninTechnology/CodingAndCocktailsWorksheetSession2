# Bonus - Media Queries
Users expect to interact with webpages using their mobile devices. Building a fully responsive webpage is not an easy undertaking, but media queries and layout systems like CSS Grid help make this faster.

{% hint style='tip' %}
##### Hey Slacker!

Remember, we're here to help.
Join the KCWiT #codingandcocktails Slack Channel: [kcwit.slack.com](http://kcwit.slack.com)
{% endhint %}

Before starting this assignment, view the completed LadyDev Bar & Grill in Chrome. Resize the browser to decrease the width. Notice regardless of the width the drinks menu and small plates menu display side to side. Let's use a media query to have the small plates menu display after the drinks menu when the width is 600px or less.

{% hint style='info' %}
Google provides breakpoints for different form factors-- dimension and resolution of the screen across different devices. 600px is a breakpoint for small devices such as small tablet or a cell phone. Learn more about [Google's responsive ui layout](https://material.io/guidelines/layout/responsive-ui.html).  
{% endhint %}


## Define grid template areas

1. Declare a grid area for the drinks menu by adding `grid-area: drinks;` to the styles for the `div` with `class="drinks"`. 
1. Declare a grid area for the Small plates menu sidebar. Name it "sidebar".  
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


## Add media query
1. Create a new style under the styles defined for `.grid-container` targeting a screen media type and a maximum width of 600px. Your style should looks like
  ```css
  @media screen and (max-width: 600px) {

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


