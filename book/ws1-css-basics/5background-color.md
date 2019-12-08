1. Select a background color for the entire page and add it to the top of _styles.css_ by using the HTML `body` selector and `background-color` property. 

   {% filename %}styles.css{% endfilename %}
    ```css
    body {
        background-color: #fefaec;
    }
    ```
    {% hint style='tip' %}
The `body` is the parent element for the website so setting a style here applies to every element within **unless** it's overridden. Organize your CSS by setting global styles at the top of the file and target styles for specific elements after global styles. Declare styles for specific elements in vertical order as it appears in the HTML to make it easy to find later.
    {% endhint %}

1. Select a background color for the Small plates menu. Notice in _index.html_ the Small plates menu `div` has a `class="sidebar"`. Create a style for this class after the style you already created for drinks and set the background color. 
   {% hint style='tip' %}
You can search for and find "Small plates" in the _index.html_ in VS Code. In the toolbar, select **Edit** ![](../images/arrow-right.svg) **Find in Files** or click on the magnifying glass on the left toolbar (where you installed Extensions). You can also use a [keyboard shortcut](../references/).
    {% endhint %}
1. To help make the navigation and footer area pop, select a background color to use. Look at the _index.html_ file to identify the selectors for the navigation and footer sections. Be sure to declare the style for the navigation bar near the top of _styles.css_ file and footer style at the bottom of the file.
   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Declare a style for <code>nav</code> after the style for <code>body</code> and add <code>background-color: #cb6f10;</code>. Declare a style for <code>footer</code> at the end of the file and add <code>background-color: #cb6f10;</code>.
</details>
   {% endhint %}

