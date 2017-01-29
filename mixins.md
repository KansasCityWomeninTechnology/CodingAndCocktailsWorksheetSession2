##Mixins

8. Let’s try a mixin now! We can use one for list styling, let’s call it list-types.

1. Create a **_mixins.scss** file in the **assets/sass** folder
1. Add your mixin to the file - this is adding a “function” to set the three properties list-style, margin and padding anytime this mixin is used in your Sass file:<br>

![](../images/image00.png)

1. In your styles.scss file replace any styling where you set those three items (likely in your navigation, product list and footer elements) with:

`@include list-reset();`

1. Save both _**mixins.scss** and **styles.scss**
1. In the command line type:

`sass assets/sass/styles.scss assets/css/styles.css`

1. Go to Chrome and refresh your page. It should again look the same. Replacing your CSS with Sass may not look very exciting but it reduces duplication in your code and makes it easier for you to change and maintain the code going forward!