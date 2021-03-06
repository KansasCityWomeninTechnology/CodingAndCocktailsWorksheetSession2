
1. Let's take care of a global setting. Remove all space around unordered lists by setting `margin` and `padding` properties to "0".
    {% hint style='tip' %}
This is the `ul` style.
    {% endhint %}

### Navigation and Footer
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

1. That looks nice. We can use the same style but for the footer by adding it as part of a selector list. Apply the same style to the footer.

   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
We can reuse the style for <code>nav li</code> by adding the <code>footer li</code> selector. The selector the style becomes <code>nav li, footer li</code>.
</details>
   {% endhint %}

1. To make the navigation list items display horizontally, add `display: inline;` to `nav li, footer li` style.

1. Add padding between the hyperlinks in the navigation bar. Declare a style for `nav a` and add the padding property there. We want 6px on the top and bottom, but 20px on the right and left. 

    {% hint style='tip' %}
Group your selectors by global to more specific. Declare the style for `nav a` before the style for `nav a:hover`.
    {% endhint %}

    {% hint style='info' %}
We can use shorthand properties to help by defining all 4 sides on the same property like this `padding: 6px 20px;`.

A commonly used mnemonic to remember the order of the values is "TROUBLE". Learn about it at [CSS-Tricks](https://css-tricks.com/remember-the-order-of-marginpadding-shorthand-with-trouble/). 

Refer to [MDN documentation for shorthand properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Shorthand_properties).
    {% endhint %}

1. Add `display: inline-block;` to `nav a` to align the hyperlinks on the same horizontal line. 

1. The `nav a` styles look mighty nice. Let's also apply it to the footer's `a` tags.

   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
We can reuse the style for <code>nav a</code> by adding the <code>footer a</code> selector. The selector the style becomes <code>nav a, footer a</code>.
</details>
   {% endhint %}

1. Give the social icons a little extra space by setting the height to 75px. Add `height: 75px;` to the existing style for `footer`.

1. One last update for the footer! The hover color for the navigation bar might look nice applied to the footer. Go ahead and apply the same style for the hover to the footer.

   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
We can reuse the style for <code>nav a:hover</code> by adding the <code>footer a:hover</code> selector. The selector the style becomes <code>nav a:hover, footer a:hover</code>.
</details>
   {% endhint %}

1. Save your file and view your page in Chrome.

### Drink menu
1. The heading for the drink menu, labeled "Menu", needs to be aligned above the drink list a little better. Looking in _index.html_ we see "Menu" is in a `h2` tag inside a `section` with `class="drinks"`. Create a selector that only changes the "Menu" text to have a 5px margin all around.

   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
We have to specify the <code>h2</code> inside the <code>class="drinks"</code> so that we don't apply the style to all <code>h2</code> elements. Target the "Menu" text only by defining styles using the selector for <code>.drinks h2</code>.
</details>
   {% endhint %}

1. The images in the drink menu are far too close the dotted top border line. Let's give it a little space by adding a 10px top padding to each drink item.

   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Define styles for each drink item using the selector for <code>.item</code>.
</details>
   {% endhint %}

1. The drink list items need a little breathing room. Add a 60px bottom margin between each drink item.

    {% hint style='working' %}
Why use margin instead of padding? Refer to the box model image in the CSS Cheat Sheet. Notice the difference where space gets added. You can see for yourself by opening Chrome DevTools, adding a bottom border and bottom padding in the **Styles** tab, and watching where space gets added. The styles you add in DevTools won't save. Mentors are here to help.  
<img src="./images/padding-vs-margin.png">
    {% endhint %}

1. We want to display the text to the right of each image. To do so, we want the image in each drink item to float to the left. Add a style to the `img` selector to `float: left`;

1. The text for the drink items are a little too close to the image. Create a little breathing room by adding a 20px margin to the right and left of the image.

   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
We can use the shortcut to add a 20px right and left margin and 0px top and bottom margin. To the style for <code>img</code>, add the <code>margin</code> property and set value to <code>0 20px</code>.
</details>
   {% endhint %}
   
