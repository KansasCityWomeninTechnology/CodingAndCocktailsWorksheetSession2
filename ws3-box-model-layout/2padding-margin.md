### Navigation bar
1. Add padding between the list items in the navigation bar by declaring a new style and adding the `padding` property to look something like
    
    {% filename %}styles.css{% endfilename %}
    ```css
    nav li {
        padding: 2px;
    }
    ```
    {% hint style='tip' %}
`padding: 2px;` means add 2px of padding on all 4 sides of the element. It's the same as 
```css
padding-top: 2px;
padding-right: 2px;
padding-bottom: 2px;
padding-left: 2px;
```
    {% endhint %}
1. To make the navigation list items display horizontally, add `display: inline;` to `nav li` style.
1. Add padding between the hyperlinks in the navigation bar. Declare a style for `nav a` and add the padding property there. We want 6px on the top and bottom, but 20px on the right and left. 

    {% hint style='info' %}
We can use shorthand properties to help by defining all 4 sides on the same property like this `padding: 6px 20px;`.

A commonly used mnemonic to remember the order of the values is "TROUBLE". Learn about it at [CSS-Tricks](https://css-tricks.com/remember-the-order-of-marginpadding-shorthand-with-trouble/). 

Refer to [MDN documentation for shorthand properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Shorthand_properties).
    {% endhint %}
1. Add `display:inline-block;` to `nav a` to align the hyperlinks on the same horizontal line. 
1. Remove all space around the navigation bar unordered list group by setting `margin` and `padding` properties to "0".
    {% hint style='tip' %}
This is the `nav ul` style.
    {% endhint %}

1. Save your file and reload your page in Chrome.

### Drink menu
1. Declare a new style for `class="drinks"` to remove the margin and padding by setting `margin` and `padding` properties to "0".
1. We want each menu item to display like a block element. To the existing style `.drinks .item` add `display: block;`.
1. The dotted top border line between the drinks menu list items is too close to the image. Add a 10px top padding to the style for `.drinks .item`
1. The drink list items need a little breathing room. Add a 60px bottom margin between each drink list item.
    {% hint style='working' %}
Why use margin instead of padding? Refer to the box model image in the CSS Cheat Sheet. Notice the difference where space gets added. You can see for yourself by opening Chrome Dev Tools, adding a bottom border and bottom padding in the **Styles** tab, and watching where space gets added. The styles you add in Dev Tools won't save. Mentors are here to help.  
<img src="./images/padding-vs-margin.png">
    {% endhint %}

1. The images in the drinks menu needs horizontal spacing by setting `margin: 0 20px;` to the existing style `.drinks img`.

### Footer
1. Remove all space around the footer unordered list group by setting margin and padding to 0. 
1. The social icons in the footer should display horizontally like it does in the navigation. Add `display: block;` to the style for the unordered list in footer. 
1. Add a style to each list item in the footer to ensure everything stays on the same horizontal line.
    {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Declare a style for the "li" tag within "footer" and add "display: inline-block;". 
</details>
   {% endhint %}
1. The social icons now extend pass the background color. Give the social icons a little extra space by setting the `footer` height to 75px by adding `height: 75px;` to the existing style for `footer`.
