###Nav Styling
Style a horizontal navigation bar (If you need some help see w3schools: [bit.ly/NavCSS](http://bit.ly/NavCSS)

1. The navigation menu is a list of links. Start by selecting the `nav` element in the _ _nav.scss_ file.

2. Set up some basic styling for the `nav` by setting the following properties:
    * `background-color`
    * `text-align` If you'd like to align your items to the right like in our sample image set this to `right`.
    * `font-family`
    * `border-bottom` You might choose to lighten or darken your background-color here by using `lighten($my-color, 10%)` to lighten it by 10% or `darken($my-color, 10%)` to darken it by 10%. A solid border would be most appropriate here.

2. The bullets on the list don't make for a visually appealing.  Since the `ul` (unordered list) element is a child of the `nav` element, nest the `ul` selector inside the `nav` element selector.  It should look something like this where the `...` ellipsis indicate code not shown in the example:

    ```sass
    nav {
        ...
        ul {
        }
    }
    ```

3. Remove the bullets from the `ul` by using the `list-style-type` property and setting it to the value `none`.  Your styling should now look something like this:

    ```sass
    nav {
        background-color: $orange;
        text-align: right;
        font-family: $body-font;
        border-bottom: 5px solid lighten($orange, 10%);
        
        ul {
            list-style-type: none;
        }
    }
    ```
    
4. 