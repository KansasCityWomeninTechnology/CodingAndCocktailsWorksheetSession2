###Normalizing
We'll start with normalizing the styling.  This is necessary to help things look consistent across browsers (ie. Microsoft Edge, Google Chrome, Internet Explorer, Safari, etc.) as each browser implements features at different times or somtimes slightly different than how the others do.  

1. If necessary, open the _ _normalize.scss_ file. 
    
2. Add the following to reset some default styles across browsers and allow a clean starting point for your styling.
    
    ```css
    /* Reset */
    html, body, div, h1, h2, h3, h4, h5, h6, p, a,
    img, ul, li, aside, footer, nav, section {
            margin: 0;
            padding: 0;
            border: 0;
            font-size: 100%;
            font: inherit;
    }
    ```
    
3. In addition set the base styling for fonts. Add the following to your _ _normalize.scss_ file underneath the closing `}` for the reset styles.  Leave a blank line between the `}` and the following styles to improve readability. Make sure you replace the variables in the example below with the colors that you've chosen and set up as variables within your project.
    
    ```css
    body {
            background-color: $cream;
            font-family: $body-font;
    }

    h1,h2,h3,h4,h5,h6 {
            color: $dark-purple;
            font-family: $header-font;
    }
    ```

