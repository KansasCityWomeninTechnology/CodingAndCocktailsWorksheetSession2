##Mixins

Let’s try a mixin now! We can use one for list styling, let’s call it `list-reset`.

1. Open the _ _mixins.scss_ file in the _sass_ folder.

2. Add your mixin to the file - this is adding a “function” to set the three properties `list-style`, `margin` and `padding` anytime this mixin is used in your Sass file:

    ```sass
    @mixin list-reset() {
        list-style-type: none;
        padding: 0;
        margin: 0;
    }
    ```

3. In your _ _nav.scss_ and _ _footer.scss_ files, replace the `list-style-type: none;` code with `@include list-reset();`

4. Save your files.

5. In the command line type `sass sass/styles.scss css/styles.css`

6. Go to Chrome and refresh your page. It should look the same but now you're consistently setting list styles across the project and have a single place to go change them should you need to in the future.

###Documentation
To understand the different CSS properties and available values visit the [Mozilla Developer Network CSS reference documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

View the Sass documentation here if you want more detailed information about how any pieces of Sass work: [bit.ly/CnCSassDoc](http://bit.ly/CnCSassDoc) 