1. Let's first clean up some spacing in the small plates section. Like the "Menu" section, we want the heading labeled "Small plates" to have a little space. To the "Small plates" header, add a margin with 5px on top and bottom, and 0px on the left and right.

   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
We have to specify the <code>h2</code> inside the <code>class="small-plates"</code>. We can use the shortcut notation to specify 5px top and bottom margin and 0px left and right margin. To the selector for <code>.small-plates h2</code> set the style <code>margin: 5px 0;</code>.
</details>
   {% endhint %}

1. Take advantage of the shorthand notation we learned to clean up the styles for `margin-top`, `margin-left`, and `margin-right` defined for the small plates list items. 

   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
<p>
    Remember the mnenomic "TROUBLE"? We can apply it here. We want 50px top, 15px right, 15px left, and 0px bottom margin. The approach is different depending on whether you used the <code>:first-child</code> pseudo class or <code>+</code> adjacent sibling combinator.
</p>

<p>
    For the pseudo class, apply the short hand <code>50px 15px 0 15px</code> to <code>margin</code>. The pseudo class will override <code>margin-top</code> from the <code>.small-plates li</code>. This is why we define the styles for the pseudo class after the style for all the elements in the list.
</p>

<p>
    For the adjacent sibling combinator, apply the short hand <code>0 15px</code> to <code>margin</code>. The style for the adjacent sibiling combinator will override <code>margin-top</code> from the <code>.small-plates li</code>. As with the psuedo class, this is why we define the style specifically for adjacent siblings after the style for all the elements in the list.
</p>
</details>
   {% endhint %}

1. Now let's use CSS Grid to align the drinks and small plates menus. In _index.html_, notice the drinks menu and small plates menu are both children of a parent `main` with `class="grid-container"`. We will target this class for grid layout. 

   In _styles.css_, declare a style for `class="grid-container"` in _styles.css_ below your styles for `class="hero"`. Add style `display: grid;`.

1. We want the drinks menu on the left with 75% width allocated to it. Drinks are, of course, most important. We want the small plates menu on the right with the remaining width allocation to it. 

   Create a grid with 2 columns with specified width by adding `grid-template-columns: 75% auto;`. Your style should look like
   
   {% filename %}styles.css{% endfilename %}
    ```css
    .grid-container {
        display: grid;
        grid-template-columns: 75% auto;
    }
    ```
1. Save your file and view in Chrome. You have two columns! ![](../images/emojis/party-popper.png)

