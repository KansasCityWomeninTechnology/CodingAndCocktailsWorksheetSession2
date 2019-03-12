1. We need a folder for the stylesheet we'll be creating tonight. In Atom, create the "css" folder for the project and create the _styles.css_ file inside the "css" folder.
   {% hint style="working" %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary> 
In Atom, right click on the "session2" project folder. Select <b>New Folder</b>. Name your folder "css". Right click on the "css" folder. Select <b>New File</b> to create your stylesheet file. Name the file <i>styles.css</i>.
</details>
   {% endhint %}

1. In Atom, open _index.html_. In the HTML `<head>` section (between the opening `<head>` and closing `</head>`), find the HTML tags for `title` and `script`. Place your cursor after the closing `title` tag, press `Enter`, and link your stylesheet by adding 

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
   {% hint style="tip" %}
Didn't have a chance to attend the HTML session or do you need a refresher? Grab a mentor and ask for an HTML overview.
   {% endhint %}

1. Save your file.

1. Now we want to preview the _index.html_ file in Chrome. Instead of saving and reloading the page manually, we'll use the atom plugin **atom-live-server**. This package opens up the web page in your default web browser and reloads the page whenever you save files. In Atom, start the live server by selecting **Packages** <i class="fa fa-long-arrow-right"></i> **atom-live-server**. Select **Start server**. A browser tab will open.
   {% hint style='danger' %}
If you don't have the **atom-live-server** package, take a moment to [set up your workspace](/setup).
   {% endhint %}   

   {% hint style='danger' %}
If the tab opens in another browser, copy the URL and paste it into a new tab in Chrome. The reload will automatically happen in Chrome.

If you get an access warning, click "Allow" to let **atom-live-server** serve the application.

If you are borrowing a laptop and get an access warning, please contact a member of the Coding & Cocktails leadership team for access.
   {% endhint %}   

   {% hint style='danger' %}
If you have more than 1 project folder open in Atom, atom-live-server will serve the _index.html_ from the first project. Remove all projects from Atom except for this session.
   {% endhint %}  

1. Take a look at your app in Google Chrome and notice the current styling. The page doesn't look good yet but we've got our initial setup for our project done. Now let's get to the fun part - styling!

