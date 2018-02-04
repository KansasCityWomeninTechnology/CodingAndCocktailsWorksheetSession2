1. In the footer, the copyright text in the `p` needs to be a contrasting color, centered, and have a bottom margin of 15px.
   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Declare a style for the "footer p" selector.

Add "color: white;" to set color. You may have a different color in mind.

Add "text-align: center;" to center.

Add "margin-bottom: 15px;" to space.
</details>
   {% endhint %}

1. The social icons are icon fonts. We can style these like they are text. Set the icons using the same contrasting color as the copyright. 
   
   {% filename %}styles.css{% endfilename %}
    ```css
    footer i {
        color: white;
    }
    ```
1. Give the icons space by setting top and bottom padding to 2px and left and right padding to 10px.
1. Center the list of icons by setting the `text-align` property in the `ul` styles.
1. Save your file and reload your page.

![](https://media.giphy.com/media/3ohhwo4PzDFaz2sADu/giphy.gif)