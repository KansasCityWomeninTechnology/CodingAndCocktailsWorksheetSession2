1. In VS Code, open _index.html_. Inside the `body` HTML tag, notice we have a variety of different HTML tags, including `img` for images. Let's try applying a style to the `img` element.

   {% hint style='tip' %}
The syntax for a CSS rule looks like this:
```css
selector {
    property: value;
}
```
   {% endhint %}

   {% hint style='working' %}
Take a moment to review _index.html_. 

In the HTML, notice we have a `nav` element for navigation, a `section` about the establishment with hero text, inside a `main` element there's 2 `section`s-- one for drinks menu and one for small plates menu, and lastly a `footer` for contact information. Inside the various `nav`, `section`, or `footer` nodes, there's elements for headers (`h1 - h6`), paragraphs (`p`), unordered lists (`ul`), images (`img`), and anchors (`a`).

Some elements have a `class` declared, such as the about `section` has `class="hero"`. We will apply CSS rules to both HTML elements and by class. 

Feel free to ask questions or talk through the layout of the HTML with your mentor.
   {% endhint %}

1. Open _styles.css_ and add the following code
    
    {% filename %}styles.css{% endfilename %}
    ```css
    img {
        width: 25%;
    }
    ```
    Save your file and view your app in Chrome. The width of all the images resized to 25% of the view. 

    {% hint style='tip' %}
VS Code can help you out! IDEs can help auto-complete code for you, including CSS properties. When you start typing a property, VS Code will suggest properties matching the name.
    {% endhint %}

1. Now let's try absolute sizes. Change your style to use `width: 120px;`. Save your file and view your app in Chrome. The width of all the images resized to 120 pixels.

    {% hint style='tip' %}
You can inspect elements in Chrome DevTools. Right click on an image and select **Inspect**. If you aren't familiar with Chrome DevTools or want a refresher, feel free to grab a mentor. Mentors love talking about **debugging**.
    {% endhint %}

1. Specify the height of your images by adding `height: 120px;`. Save your file and view your app in Chrome. The height of the images resized to 120 pixels as well. 

    {% hint style='info' %}
The images look distorted. This is because when you set height **or** width of an image, the image automatically scales and maintains [aspect ratio](https://www.w3schools.com/howto/howto_css_aspect_ratio.asp) but when you specify both height **and** width, the image resizes to the specified height and width and stretches to accommodate. 
    {% endhint %}

