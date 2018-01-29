1. Select a color that displays when your mouse hovers over the hyperlink tags in your navigation bar and footer.
1. Create a style targeting the hover Pseudo Class on the `a` tag within `nav` and define the `background-color` property. Your code should look similar to this.
    
    {% filename %}styles.css{% endfilename %}
    ```css
    nav a:hover {
        background-color: #d88731;
    }
    ```
    {% hint style='tip' %}
Group styles for the same parent element together to make it easier for yourself. Group all the `nav` style together, but order by specificity.
    {% endhint %}
    Save your file and reload in Chrome. What happens when you hover over the links in the navigation bar?

    ![](https://media.giphy.com/media/B0vFTrb0ZGDf2/giphy.gif)

1. We don't want the bullets to show in the navigation menu. Remove the bullets by setting the `list-style-type` property to "none" on the `ul` tag in `nav`. Your code should look like this.

    {% filename %}styles.css{% endfilename %}
    ```css
    nav ul {
        list-style-type: none;
    }
    ```
    Save your file and reload in Chrome. The navigation bar is starting to look better.
    {% hint sty="info" %}
Learn more about styling lists using [MDN list styling reference](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Styling_lists). 
    {% endhint %}
1. Repeat the steps in the section by adding the hover color and removing the bullets in the `footer`. Be sure to put these styles towards the bottom of the page with your footer background color.