1. In the footer, the copyright text in the `p` needs to be a contrasting color, centered, and have a bottom margin of 15px.
   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Declare a style for the <code>footer p</code> selector.

Add <code>color: white;</code> to set color. You may have a different color in mind.

Add <code>text-align: center;</code> to center.

Add <code>margin-bottom: 15px;</code> to space.
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

1. Save your file and view your page in Chrome. ![](../images/emojis/party-popper.png)

1. Share your success by posting a screenshot to Slack!  


![](https://media.giphy.com/media/3ohhwo4PzDFaz2sADu/giphy.gif)