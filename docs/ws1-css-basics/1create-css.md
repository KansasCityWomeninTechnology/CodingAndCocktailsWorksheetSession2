1. In Atom, right click on the "CSS" project folder. Select **New Folder**. Name your folder "css". This folder will house your stylesheet.
   {% hint style='danger' %}
Notice the case difference in "CSS" folder that contains all your code this session and "css" folder that contains your styles. 
	{% endhint %}

1. Right click on the "css" folder. Select **New File** to create your stylesheet file. Name the file _styles.css_.
1. In Atom, open _index.html_. In the HTML `<head>` section (between the opening `<head>` and closing `</head>`), find the HTML tags for `title` and `script`. Place your cursor after the `title` tag, press `Enter`, and link your stylesheet by adding 

   `<link rel="stylesheet" href="css/styles.css">`.
   
   The `<head>` section of your HTML should look like this:

      {% filename %}index.html{% endfilename %}
    ```html
    <head>
      <meta charset="UTF-8">
      <title>LadyDev Bar &amp; Grill</title>
      <link rel="stylesheet" href="css/styles.css">
      <script src="https://use.fontawesome.com/81b69a015b.js"></script>
    </head>
    ```

1. Save your file.
1. Open your _index.html_ file in Google Chrome and notice the current styling.  

    {% hint style='tip' %}
There's 2 different ways to open the file in Chrome. 
	
In Chrome, you can select **File** <i class="fa fa-long-arrow-right"></i> **Open File**. Navigate to your "CodingAndCocktails\CSS" folder and open the _index.html_ file. You can also use the keyboard shortcut `ctrl` + `o` on Windows machines or `cmd` + `o` on Macs.

Or you can navigate to "CodingAndCocktails\CSS" folder, right click on the _index.html_ file and choose **Open with**. Select Google Chrome from the list.
	{% endhint %}

The page doesn't look good yet but we've got our initial setup for our project done. Now let's get to the fun part - styling!

