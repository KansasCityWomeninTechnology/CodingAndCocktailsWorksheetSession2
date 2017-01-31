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
         
 3. 

###Documentation
To understand the different CSS properties and available values visit the [Mozilla Developer Network CSS reference documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

View the Sass documentation here if you want more detailed information about how any pieces of Sass work: [bit.ly/CnCSassDoc](http://bit.ly/CnCSassDoc) 
