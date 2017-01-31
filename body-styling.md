###Body Styling

1. In the project pane on the left, right click on the sass folder and select `New File`. 

2. Type `_main.scss` and press enter. This will be the partial file where the styling for the main body portion of our page will be located.

3. Don't forget to import main into your _styles.scss_ file.

2.  Start with styling the main “hero” image and text with the large page heading, a smaller “tagline” and some about text.

    1. Select the `.hero` class.
    
    2. Give it a `height:` and a `width:`.  A `600px;` height should work well. It should cover `100%;` of the width of the page.
    
    3. Instead of having an `<img>` HTML element here to display the image, we'll be using a background image on our div.  
    
        1. Take a look at the [background property documentation on MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/background).  It is a pretty powerful property with the ability to set values for multiple background properties in one.  
        
        2. Set the `background:` property to `url("../images/hero.jpg") no-repeat center top;`.  
        
        {% hint style='info' %}
        This is telling the background property that we are using a link to find our image (url = **u**niform **r**esource **l**ocator).  Go up one directory/folder from where we are (`../`), look in the images folder (`images/`) and use the `hero.jpg` file as the background image.
        
        Also we don't want to repeat the image, we just want a single image displayed (`no-repeat`).
        
        The image should be `center`ed horizontally and align the `top` of the image with the top of the background layer.
        {% endhint %}
        
        3. Finally, make sure the `background-size:` is set to `cover;` to make the image cover the width and height of the container.
        
    4. Select the `.hero-text` class and give it a `width:` of `50%;` and add a `padding-top`.  See if you can find a good value for the top padding so it doesn't sit right at the top of the page and looks nice.
    
    5. Also make sure your text is centered.  Hint: https://developer.mozilla.org/en-US/docs/Web/CSS/text-align.
    
    6. Set the `color:` and `font-size:` to appropriate values for the `h1`, `h2` and `p` elements.
    
    7. You'll also want to add some extra margin on the bottom of the `h2` element to separate it from the `p` text.

3.  Style a product list

4.  Style the sidebar Customer Favorites content to display on the right side

###Documentation
To understand the different CSS properties and available values visit the [Mozilla Developer Network CSS reference documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

View the Sass documentation here if you want more detailed information about how any pieces of Sass work: [bit.ly/CnCSassDoc](http://bit.ly/CnCSassDoc) 
