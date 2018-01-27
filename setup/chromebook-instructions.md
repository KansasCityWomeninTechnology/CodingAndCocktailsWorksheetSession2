Tonight we will use [CodePen](https://codepen.io) as your IDE.

1. Sign up for a [free account at CodePen](https://codepen.io/accounts/signup/user/free).

1. Confirm your account from your email and log in to CodePen.
   {% hint style='danger' %}
You must confirm your CodePen account to save your work and view your webpage in a separate browser tab.  
   {% endhint %}

1. Select **Create** <i class="fa fa-long-arrow-right"></i> **New Pen** from the top toolbar.

1. Select **Settings** and type in a title for this Pen, such as "Session 2". You do not need a description but feel free to add one if you'd like. Click **Save & Close**.

1. In CodePen, we have to add items to the `head` section of the HTML separately. Click the **Gear** icon next to "HTML" to open HTML settings. Add the `<meta>`, `<title>`, and `<script>` tags from the _index.html_ shown in [Create HTML file](#html-file) to the "Stuff for &lt;head&gt;" textbox. 

   The `<meta>`, `<title>`, and `<script>` tags are available in the code snippet below for your convenience.
   ```html
   <meta charset="UTF-8">
   <title>LadyDev Bar &amp; Grill</title>
   <script src="https://use.fontawesome.com/81b69a015b.js"></script>
   ```

   Click **Save & Close**.

    {% hint style='info' %}
You will need to open HTML settings to access "Stuff for &lt;head&gt;" every time the worksheet instructs you to modify the head section.
    {% endhint %}

1. Copy the contents of the `<body>` tag from the _index.html_ shown in to **HTML** pane.
   The contents of the `<body>` tag are available in the code snippet below for your convenience.
   ```html
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
                    <a href="#"><img src="https://raw.githubusercontent.com/KansasCityWomeninTechnology/CSSCompilerPractice/master/images/martini.jpg" alt=""></a>
                    <h3 class="head">Martinis</h3>
                    <p>Made with our own homemade gin and dry vermouth.  Choose from The Classic, Lemondrop, or Chocolate.</p>
                 </li>
                 <li class="item">
                    <a href="#"><img src="https://raw.githubusercontent.com/KansasCityWomeninTechnology/CSSCompilerPractice/master/images/wine.jpg" alt=""></a>
                    <h3 class="head">Wine</h3>
                    <p>There are just too many to list.  Ask your server for a recommendation.</p>
                 </li>
                 <li class="item">
                    <a href="#"><img src="https://raw.githubusercontent.com/KansasCityWomeninTechnology/CSSCompilerPractice/master/images/whiskey-cocktails.jpg" alt=""></a>
                    <h3 class="head">Whiskey cocktails</h3>
                    <p>Whiskey.  Some might consider it their spirit animal.  Thank goodness it's not just for men anymore.</p>
                 </li>
                 <li class="item">
                    <a href="#"><img src="https://raw.githubusercontent.com/KansasCityWomeninTechnology/CSSCompilerPractice/master/images/margarita.jpg" alt=""></a>
                    <h3 class="head">Margaritas</h3>
                    <p>Slushy frozen delicousness, in Peach, Strawberry, or Mango.  Served with a rock-salted rim and lime.</p>
                 </li>
                 <li class="item">
                    <a href="#"><img src="https://raw.githubusercontent.com/KansasCityWomeninTechnology/CSSCompilerPractice/master/images/hot-cocktail.jpg" alt=""></a>
                    <h3 class="head">Hot &amp; Creamy</h3>
                    <p>Just what you need to kick off a night of coding.  We offer concoctions with coffee, Kahlua, Bailey's, and more.</p>
                 </li>
                 <li class="item">
                    <a href="#"><img src="https://raw.githubusercontent.com/KansasCityWomeninTechnology/CSSCompilerPractice/master/images/beer.jpg" alt=""></a>
                    <h3 class="head">Beer</h3>
                    <p>We serve the finest microbrews from around the world.  How about a Saison, IPA, or Stout?</p>
                 </li>
                 <li class="item">
                    <a href="#"><img src="https://raw.githubusercontent.com/KansasCityWomeninTechnology/CSSCompilerPractice/master/images/milk.jpg" alt=""></a>
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
      <p>&copy; 2017 LadyDev Bar &amp; Grill</p>
      <ul>
         <li><a href="http://facebook.com/ladydevbargrill"><i class="fa fa-facebook-official fa-lg"></i></a></li>
         <li><a href="http://twitter.com/ladydevbargrill"><i class="fa fa-twitter fa-lg"></i></a></li>
         <li><a href="http://instagram.com/ladydevbargrill"><i class="fa fa-instagram fa-lg"></i></a></li>
         <li><a href="mailto:ladydevbargrill@example.com"><i class="fa fa-envelope-open-o fa-lg"></i></a></li>
      </ul>
   </footer>
   ```
   Save your file by clicking the **Save** button in the toolbar.

