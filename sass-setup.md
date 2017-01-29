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
	<link rel="stylesheet" href="assets/css/styles.css">
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
				<h1>LadyDev Bar &amp; Grill</h1>
				<h2>Making development more delicious every day!</h2>
				<p>Welcome to the LadyDev Bar &amp; Grill.  We're glad you're here!  Sit down, relax, and enjoy good drinks, good eats, and good friends.</p>
			</div>
		</div>
		<div class="flexbox">
			<div class="drinks col-1">
				<h2>Menu</h2>
				<ul class="drinks">
				    <li class="item">
				    	<a href="#"><img src="assets/images/martini.jpg" alt=""></a>
				        <h3 class="head">Martinis</h3>
				        <p>Made with our own homemade gin and dry vermouth.  Choose from The Classic, Lemondrop, or Chocolate.</p>
				    </li>
				    <li class="item">
				    	<a href="#"><img src="assets/images/wine.jpg" alt=""></a>
				        <h3 class="head">Wine</h3>
				        <p>There are just too many to list.  Ask your server for a recommendation.</p>
				    </li>
				    <li class="item">
				    	<a href="#"><img src="assets/images/whiskey-cocktails.jpg" alt=""></a>
				        <h3 class="head">Whiskey cocktails</h3>
				        <p>Whiskey.  Some might consider it their spirit animal.  Thank goodness it's not just for men anymore.</p>
				    </li>
				    <li class="item">
				    	<a href="#"><img src="assets/images/margarita.jpg" alt=""></a>
				        <h3 class="head">Margaritas</h3>
				        <p>Slushy frozen delicousness, in Peach, Strawberry, or Mango.  Served with a rock-salted rim and lime.</p>
				    </li>
				    <li class="item">
				    	<a href="#"><img src="assets/images/hot-cocktail.jpg" alt=""></a>
				        <h3 class="head">Hot &amp; Creamy</h3>
				        <p>Just what you need to kick off a night of coding.  We offer concoctions with coffee, Kahlua, Bailey's, and more.</p>
				    </li>
				    <li class="item">
				    	<a href="#"><img src="assets/images/beer.jpg" alt=""></a>
				        <h3 class="head">Beer</h3>
				        <p>We serve the finest microbrews from around the world.  How about a Saison, IPA, or Stout?</p>
				    </li>
				    <li class="item">
				    	<a href="#"><img src="assets/images/milk.jpg" alt=""></a>
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
			<li><a href="http://facebook.com/ladydevbargrill"><img src="assets/images/fb.png" alt=""></a></li>
			<li><a href="http://twitter.com/ladydevbargrill"><img src="assets/images/twitter.png" alt=""></a></li>
			<li><a href="http://instagram.com/ladydevbargrill"><img src="assets/images/instagram.png" alt=""></a></li>
			<li><a href="mailto:ladydevbargrill@example.com"><img src="assets/images/email.png" alt=""></a></li>
		</ul>
	</footer>
</body>
</html>
    ```
    
	8. Save the file.

5. Set up project structure.

	1. Right click again on that `CSS` folder in the right pane and select `New Folder`.  
	
	2. Type 'sass' and press enter.
	
	3. In the project pane on the right, right click on the sass folder and select `New File`. 

	4. Type `styles.scss` and press enter. This will be your main Sass styling file and will only contain import statements when we’re done.


