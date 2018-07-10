## Multiple columns and the grid model

File `blogdrama.html` [GitHub Source](https://github.com/tomcam/spectre-book/blob/master/examples/blogdrama.html), 
[Preview](https://htmlpreview.github.com/?https://github.com/tomcam/spectre-book/blob/master/examples/blogdrama.html)

```html
<!doctype html>
<html lang="en">
<head>
	<!-- Create title for browser tabs & Favorites -->
	<title>Blogdrama template | Spectre.css</title>
	<!-- Notify browsers this page is in Unicode -->
	<meta charset="utf-8">
	<!-- This site is responsive. Use full screen width. -->
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<meta name="description" content="2 column blog template">
	<meta name="keywords" content="spectre.css, blog, template">	
	<link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre.min.css">
	<link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre-exp.min.css">
	<link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre-icons.min.css">
	<style>
		p { font-size: 1.5em;}	
		h1 { font-size: 3em; }
		h3 { font-size: 2rem; line-height: 1em; margin-bottom: 0; }
		h1, h3 { font-weight: 700; }
		h4 { margin-bottom: 0;}
		.titlecol { height: 100vh; }		
	</style>
</head>
<body>
	<div class="container">
		<div class="columns">
			<!-- LEFT COLUMN -->
			<div class="column col-4 col-sm-12 float-right bg-dark text-light titlecol" 
				style="padding-top: 20%; padding-left: 2em; padding-right: 2em;";>
				<h3><i class="icon icon-message text-success"></i></h3>
				<div class="divider" style="padding-top: 1em;"></div>
				<h3>Notes</h3>
				<h4>From the edge</h4>
			</div><!-- .column .col-4 .col-sm-12 -->

			<!-- RIGHT COLUMN-CLIENT AREA -->
			<div class="column col-8 col-sm-12 float-left"  
				style="padding-top: 20%; padding-left: 2em;">		
				<h1 class="text-primary">Welcome, my friends.</h1> 
				<h2>Dramatic, simple 2-column responsive blog</h2>
				<p>When the web page narrows the left column 
					moves over the right column, thanks
					to <samp>col-sm-12</samp> 
					and  <samp>float-right</samp>.</p>
			</div><!-- .column .col-8 .col-sm-12 -->

		</div><!-- .columns -->
	</div><!-- .container  -->
</body>```

Here's the resulting web page:

![](screenshots/screenshot-min-1024x512.png)
