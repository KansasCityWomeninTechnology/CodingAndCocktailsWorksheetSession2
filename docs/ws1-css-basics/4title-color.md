1. Pick out a color palette to use from [http://colorhunt.co](http://colorhunt.co). Make note of the hex color values displayed when you hover over each color in your chosen palette. 
    {% hint style='tip' %}
Ensure your colors are a11y friendly by using the WebAIM [Color Contrast Checker](https://webaim.org/resources/contrastchecker/). You can input your selected foreground and background colors to find contrasting colors that improve legibility.

Google's [Color Tool](https://material.io/color/) makes this a little easier by pre-defining color palettes with accessible contrast.
    {% endhint %}

1. In Atom, find the `div` containing the HTML header tag with the text "LadyDev" in _index.html_. Note the `div` has `class="hero-text"` and you have `h1`, `h2`, and `p` tags to style.

1. In _styles.css_, declare a style for the `h1` tag above the existing style for `.drinks img` and add the color you selected for the title using the `color` property like this
    
    {% filename %}styles.css{% endfilename %}
    ```css
    .hero h1 {
        color: #cb6f10;
    }
    ```

1. Repeat to create styles targeting `h2` and `p` right after your `.hero h1` style and apply the same color.
    {% hint style='working' %}
What happens if you don't specify class when styling the `p` element? 

The color changes applies to all `p` elements on the page, not just the title. Try it yourself to see CSS specificity.
    {% endhint %}

1. Save your file and view your page in Chrome.
    {% hint style='tip' %}
Save your _styles.css_ file and view your app often so you can see the changes as we go along. The worksheet will call out specific places to save and view the web page to illustrate a concept, but feel free to save and view your page as often as you want. It helps to see the changes as your write your CSS.   
    {% endhint %}
