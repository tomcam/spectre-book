# Timelines

A timeline requires at a minimum:

* A div of class `timeline`
  * Nested in the div of class `timeline` are one or more divs of time `timeline-item`
    * Nested in the div of class `timeline-item` is an icon of class `timeline-icon` for the timeline circle, which may be an active link
    * Following the icon is a div of type `timeline-content`.
      * Nested in the `timeline-content` div is a div of type `tile`.
        * Nested in the `tile` div is an item, for example a `<p>` tag, of class `tile-title` or `tile-subtitle`

Timelines are in the "experimental" class (which has been stable and usable for more than 2 years), so they require
the `spectre-exp.min.css` style sheet.

## Example 1: The minimal timeline (one item)

The first example is a timeline with one tickmark and a single item describing that tickmark.


```html{17-28}
<!doctype html>                                                                                                                                            
<html lang="en">                                                                                                                                           
<head>                                                                                                                                                     
                                                                                                                                                           
        <!-- Create title for browser tabs & Favorites -->                                                                                                 
        <meta charset="utf-8">                                                                                                                             
        <!-- This site is responsive. Use full screen width. -->                                                                                           
        <meta name="viewport" content="width=device-width, initial-scale=1.0">                                                                             
        <title>Minimal timeline | Spectre.css</title>                                                                                                      
        <link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre.min.css">                                                                  
        <!-- Considered an "experimental" feature -->                                                                                                      
        <link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre-exp.min.css" />                                                            
                                                                                                                                                           
</head>                                                                                                                                                    
<body>                                                                                                                                                     
<div class="container">                                                                                                                                    
        <div class="timeline">                                                                                                                             
                <div class="timeline-item">                                                                                                                
                        <div class="timeline-left"><a class="timeline-icon" href="#"></a></div><!-- .timeline-left -->                                     
                        <div class="timeline-content">                                                                                                     
                                <div class="tile">                                                                                                         
                                        <div class="tile-content">                                                                                         
                                                <p class="tile-title">Item 1 (title)</p>                                                                   
                                        </div><!-- .tile-content -->                                                                                       
                                </div><!-- tile -->                                                                                                        
                        </div><!-- .timeline-content -->                                                                                                   
                </div><!--.timeline -item -->                                                                                                              
        </div><!-- .timeline -->                                                                                                                           
</div><!-- .container -->                                                                                                                                  
</body> 
```

File `timeline-minimal.html` [GitHub Source](https://github.com/tomcam/spectre-book/blob/master/code/timeline-minimal.html), 
[Preview](https://htmlpreview.github.com/?https://github.com/tomcam/spectre-book/blob/master/code/timeline-minimal.html)

## Example 2: A timeline with three items on one tickmark

Here's a timeline with one tickmark on the time line consisting of three items

File `timeline-minimal-with-subtitle.html` [GitHub Source](https://github.com/tomcam/spectre-book/blob/master/code/timeline-minimal-with-subtitle.html), 
[Preview](https://htmlpreview.github.com/?https://github.com/tomcam/spectre-book/blob/master/code/timeline-minimal-with-subtitle.html)

```html
<!doctype html>
<html lang="en">
<head>

	<!-- Create title for browser tabs & Favorites -->
	<meta charset="utf-8">
	<!-- This site is responsive. Use full screen width. -->
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Minimal timeline | Spectre.css</title>
	<link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre.min.css">
	<!-- Considered an "experimental" feature -->
	<link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre-exp.min.css" />
	
</head>
<body>
<div class="container">
	<div class="timeline">
		<div class="timeline-item">
			<div class="timeline-left"><a class="timeline-icon" href="#"></a></div><!-- .timeline-left -->
			<div class="timeline-content">
				<div class="tile">
					<div class="tile-content">
						<p class="tile-title">Item 1 (title)</p>
						<p class="tile-subtitle">Item 2 (subtitle)</p>
						<p class="tile-subtitle">Item 3 (subtitle)</p>
					</div><!-- .tile-content -->
				</div><!-- tile -->
			</div><!-- .timeline-content -->
		</div><!--.timeline -item -->
	</div><!-- .timeline -->
</div><!-- .container -->
</body>
```
