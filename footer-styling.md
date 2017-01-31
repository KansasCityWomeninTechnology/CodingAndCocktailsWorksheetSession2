##Footer Styling
Style a footer with copyright information and social media links.

1. Select the `footer` element and set some basic styling by giving values to the following properties:

    * `background-color:` using one of the color variables from your selected color palette.
    
    * `border-top` (Use lighten or darken here again!)
    
    * `height` to give it enough room for the content.  `75px;` would be a good value here.
    
2. Style the copyright text inside the footer.  Select the `p` (paragraph) element nested inside the `footer` element selector.  That means it looks like this (missing the properties you set in step 1):
    
     ```sass
     footer {
         p {
         }
     }
     ``` 
     
     1. Set the following properties for the `p` element:
         
         * `margin-bottom: 15px;` to space out the paragraph text from the social media below.
         * `text-align:` if you want to center the text set it to `center;`
         * `color:` to specify the text color.
         
3. Make sure the social media font-awesome icons are styled as well.  They're set up in a list and again, we don't want bullets on our list.
    
    1. Select the `ul` (unordered list) element and set the `list-style-type`, `text-align` properties appropriately.
    
    2. Set the `display:` property to `block;`.
    
4. To align the icons in a row, select the `li` (list item) elements and set their `display` property to `inline-block;`.

5. A few last adjustments include adding some spacing around the icons and changing their color.  

    1. Select the `i` (icon) element and set the `padding:` property to `2px 10px;`.
    
    2. Change the color to one from your palette.
    
6. Now compile the Sass into CSS. 
    
    1. In the command line (Git Bash for windows, iTerm2 for macs) make sure you are in the folder containing your _index.html_ file.
    
    2.  Type: `sass sass/styles.scss css/styles.css`

7. Go to Google Chrome and refresh your page. You should have a more visually appealing footer now.



###Documentation
To understand the different CSS properties and available values visit the [Mozilla Developer Network CSS reference documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

View the Sass documentation here if you want more detailed information about how any pieces of Sass work: [bit.ly/CnCSassDoc](http://bit.ly/CnCSassDoc) 
