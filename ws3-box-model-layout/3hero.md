1. Open _index.html_ and find the `div` containing the title of the web page. Because we want our hero image to fill the entire title area, declare a style for `class="hero"` in _styles.css_.
1. Add a background image to the style using 
   ```css
   background: url("https://raw.githubusercontent.com/KansasCityWomeninTechnology/CSSCompilerPractice/master/images/hero.jpg") no-repeat center top;
   ```
   Save your file and refresh your page. 

   ![](https://media.giphy.com/media/l44QiZECjPEjLAwzm/giphy.gif)

   Yay! A hero image! But it's cut off. Let's resize it.
    {% hint style='info' %}
Why did we have to add `no-repeat center top` to the image? We used shorthand properties to specify the image shouldn't repeat, center the image, and display image from top.

Refer to [MDN documentation for background property](https://developer.mozilla.org/en-US/docs/Web/CSS/background).
    {% endhint %}
1. In the same style above the "background" property, define the size of the `div` for `class="hero"` by setting `height: 600px;`. This sets the size for the div, but now we need to specify the background image should resize. Add `background-size: cover;` to the same style after the background image.
{% hint style='info' %}
Refer to [MDN documentation for background-size property](https://developer.mozilla.org/en-US/docs/Web/CSS/background-size).
    {% endhint %}

1. Add some space after the `h2` element in the hero by setting bottom margin to 20px;






