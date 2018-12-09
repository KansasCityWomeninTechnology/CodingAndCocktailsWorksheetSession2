
1. Open Atom from your installed applications. In Atom, select **File** <i class="fa fa-long-arrow-right"></i> **Add project folder**.

1. Navigate to and select the "CodingAndCocktails/session2" folder.
   {% hint style='danger' %}
If you don't have a "CodingAndCocktails/session2" directory, take a moment to [set up your workspace](/setup).
   {% endhint %}  

1. In the **Project** pane in Atom, right click on the "session2" project folder and select **New file**.

1. Name the file _index.html_ and press `Enter` to save it in your "CodingAndCocktails/session2" folder.

1. Copy and paste the following HTML code into your _index.html_ file.
  
   {% filename %}index.html{% endfilename %}
    ```html
<!DOCTYPE html>
<html lang="en">
   <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1">
      <title>LadyDev Bar &amp; Grill</title>
      <script src="https://use.fontawesome.com/81b69a015b.js"></script>
   </head>
   <body>
      <nav class="navbar">
         <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#menu">Menu</a></li>
            <li><a href="#contact">Contact</a></li>
         </ul>
       </nav>
       <div>
          <div class="hero" id="about">
             <div class="hero-text">
                <h1>LadyDev</h1>
                <h1>Bar &amp; Grill</h1>
                <h2>Making development more delicious every day!</h2>
                <p>Welcome to the LadyDev Bar &amp; Grill.  We're glad you're here!</p>
                <p>Sit down, relax, and enjoy good drinks, good eats, and good friends.</p>
             </div>
          </div>
          <div class="grid-container" id="menu">
             <div class="drinks">
                <h2>Menu</h2>
                <ul class="drinks">
                   <li class="item">
                      <a href="#"><img src="images/martini.jpg" alt=""></a>
                      <h3 class="head">Martinis</h3>
                      <p>Made with our own homemade gin and dry vermouth.  Choose from The Classic, Lemondrop, or Chocolate.</p>
                   </li>
                   <li class="item">
                      <a href="#"><img src="images/wine.jpg" alt=""></a>
                      <h3 class="head">Wine</h3>
                      <p>There are just too many to list.  Ask your server for a recommendation.</p>
                   </li>
                   <li class="item">
                      <a href="#"><img src="images/whiskey-cocktails.jpg" alt=""></a>
                      <h3 class="head">Whiskey cocktails</h3>
                      <p>Whiskey.  Some might consider it their spirit animal.  Thank goodness it's not just for men anymore.</p>
                    </li>
                    <li class="item">
                       <a href="#"><img src="images/margarita.jpg" alt=""></a>
                       <h3 class="head">Margaritas</h3>
                       <p>Slushy frozen delicousness, in Peach, Strawberry, or Mango.  Served with a rock-salted rim and lime.</p>
                    </li>
                    <li class="item">
                       <a href="#"><img src="images/hot-cocktail.jpg" alt=""></a>
                       <h3 class="head">Hot &amp; Creamy</h3>
                       <p>Just what you need to kick off a night of coding.  We offer concoctions with coffee, Kahlua, Bailey's, and more.</p>
                    </li>
                    <li class="item">
                       <a href="#"><img src="images/beer.jpg" alt=""></a>
                       <h3 class="head">Beer</h3>
                       <p>We serve the finest microbrews from around the world.  How about a Saison, IPA, or Stout?</p>
                    </li>
                    <li class="item">
                       <a href="#"><img src="images/milk.jpg" alt=""></a>
                       <h3 class="head">Non alcoholic</h3>
                       <p>We have plenty of NA options available to quench your thirst, like lemonade, milk or soda.</p>
                    </li>
                 </ul>
              </div>
              <div class="sidebar">
                 <h2>Small plates</h2>
                 <ul class="food">
                    <li>Grassfed beef sliders</li>
                    <li>Spicy calamari</li>
                    <li>Coconut shrimp</li>
                    <li>Veggie spring rolls</li>
                    <li>Deviled eggs</li>
                    <li>Tuscan bean dip</li>
                    <li>Chicken lettuce wraps</li>
                 </ul>
              </div>
           </div>
        </div>
        <footer id="contact">
           <p>&copy; 2019 LadyDev Bar &amp; Grill</p>
           <ul>
              <li><a href="http://facebook.com/ladydevbargrill"><i class="fa fa-facebook-official fa-lg"></i></a></li>
              <li><a href="http://twitter.com/ladydevbargrill"><i class="fa fa-twitter fa-lg"></i></a></li>
              <li><a href="http://instagram.com/ladydevbargrill"><i class="fa fa-instagram fa-lg"></i></a></li>
              <li><a href="mailto:ladydevbargrill@example.com"><i class="fa fa-envelope-open-o fa-lg"></i></a></li>
            </ul>
         </footer>
      </body>
   </html>
   ```

1. Save the file by selecting **File** <i class="fa fa-long-arrow-right"></i> **Save**. ou can also use the keyboard shortcut `ctrl + s` on Windows or `cmd + s` on Mac. Unsaved files in Atom have a little blue dot on tab.

   ![](images/atom.png)

1. Now we'll prepare the images. First we need a folder for the images. In Atom, right click on the "session2" folder in the **Project** pane and select **New Folder**. Name the folder "images".

1. In Chrome, open a new tab to our GitHub repository at [https://github.com/KansasCityWomeninTechnology/CSSCompilerPractice/tree/master/images](https://github.com/KansasCityWomeninTechnology/CSSCompilerPractice/tree/master/images). 

1. Click on each image filename to view the file. Then, click the "Download" button in the upper right corner above the displayed image.
   
   ![](images/download.png)

1. Save the files into your "images" folder. 
	
	When you're done, your "images" folder should contain:
	```
	beer.jpg
	hero.jpg
	hot-cocktail.jpg
	margarita.jpg
	martini.jpg
	milk.jpg
	whiskey-cocktails.jpg
	wine.jpg
	```

Congratulate your neighbors for getting all the HTML setup done. Break the ice by asking your neighbor "What's the most embarrassing fashion trend you used to rock"?