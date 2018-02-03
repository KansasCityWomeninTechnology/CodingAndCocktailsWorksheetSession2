1. Open _index.html_ and find "Small plates" so that you know how to target styles for this list. Notice this section has `class="sidebar"`. We will target this class for styling. 
1. Remove the bullet points in the `ul` in `class="sidebar"`.  
    {% hint style='tip' %}
Remember, styles for `class` has `.` prepended. Take a look at your fine work resizing the drink menu images. 
    {% endhint %}

1. We want to add extra space between each list item on the "Small plates" menu by setting the `margin-top` property to "50px" on the list items. Create a style targeting `li` within the `ul` with `class="sidebar"` like this

   {% filename %}styles.css{% endfilename %}
   ```css
    .sidebar ul li {
       margin-top: 50px;
    }
   ```
     {% hint style='info' %}
You are using the "Descendant combinator". A combinator is a special selector. The descendant combinator contains 2 or more selectors with a space between each selector. The first selector is an ancestor of the second in the HTML. So in this case, you are saying 

_For all HTML elements with the class `.sidebar` that has a descendant `ul` that has a descendant `li`, add a top margin._
    {% endhint %}

1. Save your file and reload in Chrome. You now have plenty of spacing between each food menu item but the `margin-top` property also added space between the "Small plates" header and list. Let's take care of that extra space next.

1. Create another style targeting the `li` elements in the "Small plates" menu after the one you created in the previous step. Add the Pseudo Class `first-child` and define the `margin-top` property using the value "0". We are overriding the previous style selectively for the first child. Your code should look like this

  {% filename %}styles.css{% endfilename %}
    ```css
    .sidebar ul li:first-child {
        margin-top: 0;
    }
    ```
    Save your file and refresh the page. The spacing looks better now. 
  {% hint style='info' %}
You can also use combinators to declare a property on all `li` except the first in one fell swoop. Instead of having a style for all list items and overriding the first child, you could have written 
```css
.sidebar ul li + li {
    margin-top: 50px;
}
```

The `+` is the "Adjacent Sibiling" combinator and selects `li` elements directly after the first one. So in this case, you are saying

_For all HTML elements with the class `.sidebar` with a descendant `ul`-- apply a top margin to `li` tags declared directly after a `li` tag._

Read more about the [Adjacent sibling combinator](https://developer.mozilla.org/en-US/docs/Web/CSS/Adjacent_sibling_selectors). 
    {% endhint %}