##Sass

###Variables
1. Start by creating some Sass variables that will represent the colors in the color palette that you selected earlier.

    1. If needed, open the _variables.scss file by double clicking on it in the left pane. 
    
    2. Create your first variable for the main color of your site. Variables start with a `$` followed by the variable name.  It might look something like the following:
    
    ```
    $pink: #F9A1BC;
    ```
    
    3. Create variables for the remaining colors in your site.  It is common to name your color variables according the color name.  Things like `$turquoise`, `$white`, `$dark-purple`, etc.
    
    
###Normalizing
1. We'll start with normalizing the styling.  This is necessary to help things look consistent across browsers (ie. Microsoft Edge, Google Chrome, Internet Explorer, Safari, etc.) as each browser implements features at different times or somtimes slightly different than how the others do.  

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

###Fonts
1. Add fonts for your page.
        
        1. Back in Google Fonts ([fonts.google.com](https://fonts.google.com/)), make sure you have at least two fonts selected, one to use for headers and one to use for body text. 

        2. This time we'll find the `import` way of embedding the fonts.
        
        3. Copy the import statement for your fonts and paste it as the first line in your _styles.scss_ file.
        
        4. In the _ _variables.scss_ file, set up the variables for `$body-font` and `$header-font` referencing the Google Fonts font-families.  For example one variable might look like: `$body-font: "Work Sans", Arial, Helvetica, sans-serif;
        
        {% hint style='tip' %}
        If you select a font that is two words you'll need to wrap that in quotation marks.
        
        Often you'll want to provide backup fonts for the page to fall back on in case it can't load the chosen font.  A common fallback for sans-serif fonts might include Arial, Helvetica, sans-serif.  For serif fonts it might include "Times New Roman", Times, serif as backups.
        {% endhint %}

2. Save the _ _variables.scss_, _ _styles.scss_, and _ _normalize.scss_ files.

3. Now compile the Sass into CSS. In the command line (Git Bash for windows, iTerm2 for macs) make sure you are in the folder containing your _index.html_ file.  Type: `sass sass/styles.scss css/styles.css`

4. Go to Google Chrome and refresh your page. You should notice the font styling has changed and maybe some of the page spacing.



7. Use nesting to simplify your stylesheet - remember not to go more than 3-4 levels deep though!

1. In places where you have parent-child selectors, nest the child selectors inside the parent class or element.
1. For example instead of:<br>
![](../images/image05.png)
You might have this:<br>
![](../images/image01.png)

That way you don’t have to repeat nav in front of the child ul and li elements. Similar to the way you nest your html elements you can now organize your Sass file with nesting.

1. Save the Sass files.
1. In the command line type

`sass assets/sass/styles.scss assets/css/styles.css`

1. Open up your **assets/css/styles.css** file in Sublime Text and notice how the nested sass compiles to the parent-child selectors.
1. Go to Chrome and refresh your page. It should still look the same.




10. Feel free to try out any more of the Sass concepts we discussed tonight using the same process.


1. Compare your **styles.sass** with our answer key here: [bit.ly/CnCSassKey](https://www.google.com/url?q=http://bit.ly/CnCSassKey&sa=D&ust=1478381675890000&usg=AFQjCNHy8sjHANATp6X20-ZMCmis6PP5pw). It may not be exact but will give you an idea on what your Sass may look like.

**Congratulations! You’ve just styled a webpage using a CSS Compiler!**

