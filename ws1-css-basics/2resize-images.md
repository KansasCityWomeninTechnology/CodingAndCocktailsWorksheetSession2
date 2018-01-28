1. In Atom, open _index.html_. Find the `div` for drinks with title "Menu". It contains an unordered list with `class="drinks"` and has an image using `img` tag. We will need to apply a style to the `img` selector within `class="drinks"`.
   {% hint style='tip' %}
The syntax for a CSS rule looks like this:
```css
selector {
    property: value;
}
```
`class` attributes have `.` prepended to the selectors while `id` attributes have `#` prepended to the selectors.

To target selectors within a `class` you have to specify both the `class` and selector in your style.
    {% endhint %}
1. Open _styles.css_ and add the following code
    
    {% filename %}styles.css{% endfilename %}
    ```css
    .drinks img {
        width: 25%;
    }
    ```
    Save your file and reload your page in Chrome. The width of all the images within `class="drinks"` resized to 25% of the view. 
1. Now let's try absolute sizes. Change your style to use `width: 120px;`. The width of all the images resized to 120 pixels.
    {% hint style='tip' %}
You can inspect elements in Chrome using Dev Tools. Right click on an image and select **Inspect**. 
    {% endhint %}
1. Specify the height of your images by adding `height: 120px;`. The height of the images resized to 120 pixels as well. 
    {% hint style='info' %}
The images look distorted. This is because when you set height or width of an image, the image automatically scales and maintains [aspect ratio](https://www.w3schools.com/howto/howto_css_aspect_ratio.asp) but when you specify both height and width, the image resizes to the specified height and width and stretches to accommodate. 
    {% endhint %}

