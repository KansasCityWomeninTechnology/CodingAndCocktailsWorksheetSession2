### Navigation text 
1. The navigation text should be right aligned. In the `nav` style, add `text-align: right;`.

1. The navigation text in the hyperlink doesn't stand out enough. Let's make the following changes to the existing style for navigation hyperlinks using the existing style created for `nav a`:
   1. Change the color using an a11y friendly contrasting color by setting `color` property.
   1. Make the text bold using `font-weight: bold;`.
   1. Remove the hyperlink underline using `text-decoration: none;`.
   1. Increase text size using `font-size: 1.5em;`.
   {% hint style='info' %}
Why use `em` instead of `px` for font size? `em` is a calculated font size based off of the parent's font value. Read more about the different ways to set font size in "Possible approaches" section of [MDN documentation on font size](https://developer.mozilla.org/en-US/docs/Web/CSS/font-size).
    {% endhint %}

### Hero text
1. The header and paragraph text are too small. Let's increase text for each header and paragraph selectively using styles you already have for `class="hero"`. 
    1. Set `font-size` to 5em for `h1`.
    1. Set `font-size` to 1.5em for `h2`.
    1. Set `font-size` to 1.25em for `p`.

1. We need to apply a style to all the hero text. In _index.html_, notice a `div` with `class="hero-text"` wraps all tags for the hero text. We will target this class. 
   1. Create a style for this class and add top padding of 125px.
   1. Allocate 50% of the width of the background image by adding `width: 50%;`. 
   1. Align text to center of the `div` by adding `text-align: center;`.

### Drink menu
1. The "Menu" text in the header tag needs to be larger. Create a style targeting the `h2` header in `class="drinks"` and set font size to 3em. Add a 5px margin to give it a little space.

1. Each menu item needs to be a little larger. The header for each menu item has `class="head"`. Create a style targeting this class within drinks menu and set font size to 2em.
   {% hint style='working' %}
Create a style for `.drinks .head` to set the font size.
   {% endhint %}

1. Increase the size of each menu item description. Create a style for `.drinks p` and set font size to 1.3em.   

1. We want the image for the drinks to display on the same row as the text but along its left side. Add `float: left;` to the styles you already have for drink menu images. 
   {% hint style='info' %}
Prior to systems like Flexbox or CSS Grid, layout relied on float. Within a small container, the overhead for a layout system isn't always necessary. Read more at [MDN documentation on float](https://developer.mozilla.org/en-US/docs/Web/CSS/float).
    {% endhint %}

### Small plates menu
1. Set font size to the existing style for `class="sidebar"` to 1.5em.

1. The "Small plates" text in the `h2` tag needs to be 2em, centered, and spaced with 5px margin on the top and bottom, but no margin on the sides. Based on what we learned tonight, can you apply these styles? 
  {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Declare a style for <code>.sidebar h2</code>.

Add <code>font-size: 2em;</code> to set size.

Add <code>text-align: center;</code> to center.

Add <code>margin: 5px 0;</code> to space.
</details>
   {% endhint %}
  
