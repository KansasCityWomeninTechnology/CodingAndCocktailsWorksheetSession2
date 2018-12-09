1. In _index.html_, notice the drinks menu and small plates menu are both children of a parent `div` with `class="grid-container"`. We will target this class for grid layout. 

   Declare a style for `class="grid-container"` in _styles.css_ below your styles for `class="hero"`. Add style `display: grid;`.

1. We want the drinks menu on the left with 75% width allocated to it. Drinks are, of course, most important. We want the small plates menu on the right with the remaining width allocation to it. 

   Create a grid with 2 columns with specified width by adding `grid-template-columns: 75% auto;`. Your style should look like
   
   {% filename %}styles.css{% endfilename %}
    ```css
    .grid-container {
        display: grid;
        grid-template-columns: 75% auto;
    }
    ```
1. Save your file and view in Chrome. Tada! 🎉 You have two columns!!

