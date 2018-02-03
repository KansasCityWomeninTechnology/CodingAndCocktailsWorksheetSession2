1. Open _index.html_ and find the `div` containing the text for title of the web page. Because we want our hero image to fill the entire title area, declare a style for `class="hero"` and set `height: 600px;` in _styles.css_ like this

   {% filename %}styles.css{% endfilename %}
   ```css
   .hero {
      height: 600px;
   }
   ```
1. Add a background image to the style you created in the previous step by adding 
   ```css   
      background: url("https://raw.githubusercontent.com/KansasCityWomeninTechnology/CSSCompilerPractice/master/images/hero.jpg") no-repeat center top;
   ```
   Save your file and refresh your page. 

   ![](https://media.giphy.com/media/l44QiZECjPEjLAwzm/giphy.gif)

   Yay! A hero image! But we want it to expand across the entire width of the page. Let's resize it.
    {% hint style='info' %}
Why did we have to add `no-repeat center top` to the image? We used shorthand properties to specify the image shouldn't repeat, center the image, and display image from top.

Refer to [MDN documentation for background property](https://developer.mozilla.org/en-US/docs/Web/CSS/background).
    {% endhint %}
1. In the same style for `class="hero"`, add `background-size: cover;` after the `background` property.
{% hint style='info' %}
Refer to [MDN documentation for background-size property](https://developer.mozilla.org/en-US/docs/Web/CSS/background-size).
    {% endhint %}

1. Add some space after the `h2` element in `class="hero"` by setting bottom margin to 20px to the existing style.
   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Add "margin-bottom: 20px;" to the existing style ".hero h2". 
</details>
   {% endhint %}






