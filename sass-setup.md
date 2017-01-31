###Setup

1. In your `CodingAndCocktails` folder in your home directory create a `CSS` folder

2. Open Atom and set up your HTML file.

    1. Close any open tabs by hovering over them with your mouse at the top of the screen and clicking on the small x that appears.
    
    2. In the `File` menu choose `Add Project Folder...`
    
    3. Navigate to the `CSS` folder you just created in step 1 and choose `Open`.
    
    4. You should now have a pane on the left displaying the `CSS` folder. Right click on the folder and choose `New File`.
    
    5. Type _index.html_ and press enter.
    
    6. A new file should display on the left and should open in your main work area.  
    
    7. Copy and paste the following HTML code into your _index.html_ file.

    ```html
    <!DOCTYPE html>
<html lang="en">
		<head>
			<meta charset="UTF-8">
			<title>LadyDev Bar &amp; Grill</title>
			<link rel="stylesheet" href="css/styles.css">
			<script src="https://use.fontawesome.com/81b69a015b.js"></script>
		</head>
		<body>
			<nav class="navbar">
				<ul id="drinks">
					<li><a href="#">Home</a></li>
					<li><a href="#about">About</a></li>
					<li><a href="#drinks">Menu</a></li>
					<li><a href="#contact">Contact</a></li>
				</ul>
			</nav>
			<div class="main">
				<div class="hero" id="about">
					<div class="head">
						<div class="hero-text">
							<h1>LadyDev</h1>
							<h1>Bar &amp; Grill</h1>
						</div>
						<h2>Making development more delicious every day!</h2>
						<p>Welcome to the LadyDev Bar &amp; Grill.  We're glad you're here!</p>
						<p>Sit down, relax, and enjoy good drinks, good eats, and good friends.</p>
					</div>
				</div>
				<div class="flexbox">
					<div class="drinks col-1">
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
					<div class="food sidebar col-2">
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
		</body>
</html>
    ```
    
	8. Save the file.

3. Set up project structure.

	1. Right click again on that `CSS` folder in the left pane and select `New Folder`.  
	
	2. Type 'sass' and press enter.
	
	3. Right click again on that main `CSS` folder in the left pane and select `New Folder`.  
	
	4. Type 'css' and press enter.
	
	5. In the project pane on the left, right click on the `sass` folder and select `New File`. 

	6. Type `styles.scss` and press enter. This will be your main Sass styling file and will only contain import statements when we’re done.
	
	7. In the project pane on the left, right click on the sass folder and select `New File`. 

	8. Type `_variables.scss` and press enter. This will be the file where all of our variables that we use in our project will be located.
	
	9. Repeat the process to create additional files to hold our partials for the different areas of our website.  Create files in the `sass` folder called _ _nav.scss_, _ _main.scss_, _ _footer.scss_, _ _normalize.scss_, and _ _mixins.scss_.

	10. Open the _styles.scss_ file by double clicking on it in the left pane if it is not already open.  You’ll need to import the partial files so type in `@import “variables”;` to import the _ _variables.scss_ file.  Add import statements for the rest of the files as well.  Your _styles.scss_ file should look like this when you're done: 
	
	```scss
	@import "variables";
	@import "normalize";
	@import "mixins";
	@import "nav";
	@import "main";
	@import "footer";
	```
	
4. Open your _index.html_ file in Google Chrome and notice the current styling.  You can do this two ways.
	
	1. Open Google Chrome. 
		
		1. From the `File` menu choose `Open File...`.
		
		2. Navigate to find your _index.html_ file and choose `Open`.
		
	2. In your File Explorer (windows) or Finder (macs) navigate to your folder containing the _index.html_ file.
	
		1. Right click on the file and choose `Open with`.
		
		2. Choose Google Chrome from the list.

We've got our initial setup for our project done, now let's get to the fun part - styling!

###Documentation
To understand the different CSS properties and available values visit the [Mozilla Developer Network CSS reference documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

View the Sass documentation here if you want more detailed information about how any pieces of Sass work: [bit.ly/CnCSassDoc](http://bit.ly/CnCSassDoc) 

