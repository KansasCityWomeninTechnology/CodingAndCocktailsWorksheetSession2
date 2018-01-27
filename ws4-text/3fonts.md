### Navigation text 
1. The navigation text should be right aligned. In the `nav` style, add `text-align: right;`.
1. The navigation text in the hyperlink doesn't stand out enough. Let's make the following changes to the existing style for navigation hyperlinks:
   1. Change the color using an a11y friendly contrasting color by setting `color` property.
   1. Make the text bold using `font-weight: bold;`
   1. Remove the hyperlink underline using `text-decoration: none;`
   1. Increase text size using `font-size: 1.5em;`

### Hero text
1. We need to apply a style to all the hero text. In _index.html_, notice a `div` with `class="hero-text"` wraps all tags for the hero text. We will target this class. 
   1. Create a style for this class and add top padding of 125px;
   1. Allocate 50% of the width of the background image by adding `width: 50%;`. 
   1. Align text to center of the div by adding `text-align: center;`.
1. The header and paragraph text are too small. Let's increase text for each header and paragraph selectively. 
    1. Set "font-size" to 5em for `h1`.
    1. Set "font-size" to 1.5em for `h2`.
    1. Set "font-size" to 1.25em for `p`.

### Drink menu
1. The "Menu" text in the header tag needs to be larger. Create a style targeting this header and set font size to 3em. Add a 5px margin to give it a little space.
1. Each menu item needs to be a little larger. The header for each menu item has `class="head"`. Create a style targeting this class within drinks menu and set font size to 2em.
1. Increase the size of each menu item description in the `p` tag by setting font size to 1.3em.   
1. We want the image for the drinks to display on the same row as the text. Add `float: left;` to the styles for the images. 

### Small plates menu
1. Set font size for the enter section to 1.5em.
1. The "Small plates" text in the header tag needs to be 2em, centered, and spaced with 5px margin on the top and bottom, but no margin on the sides. 
  {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Declare a style for the h2 tag within class="sidebar".
Add "font-size: 2em;" to set size.
Add "text-align: center;" to center.
Add "margin: 5px 0;" to space.
</details>
   {% endhint %}
  
