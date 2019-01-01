1. Select a border color to use between the navigation bar and menu. We'll use the same border color between the menu and the footer.

1. In the style definition for `nav`, add a property for the bottom border and set your selected color as the background. The property will look like `border-bottom: 5px solid #f1a250;`.

1. Repeat for the `footer` except use a top border.
   {% hint style='tip' %}
The top border property is `border-top`.
   {% endhint %}

1. Turn your attention towards the drink menu. Create a style for `class="drinks"` and remove the bullets.

1. Define borders between each drink in the drink menu by adding a top border to each item in the list. Target both the `.drinks` and `.item` classes in your style and set a thin dotted line. The style will look like
    
    {% filename %}styles.css{% endfilename %}
    ```css
    .drinks .item {
        border-top: 1px dotted #637056;
    }
    ```
1. Add a border radius to the images in the drink menu. Add this new property to the existing style you already created to resize the images. By setting the value "50%", you make a circular border around the image. 
  {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
We already have a style declared for <code>.drinks img</code>. Add <code>border-radius: 50%;</code> to it. 
</details>
   {% endhint %}
    
1. Save your file and view in Chrome. Looking good!