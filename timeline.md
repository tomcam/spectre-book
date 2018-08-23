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

```html
<!doctype html>
<html lang="en">
<head>
	<!-- Create title for browser tabs & Favorites -->
	<meta charset="utf-8">
	<!-- This site is responsive. Use full screen width. -->
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Minimal timeline with 1 tickmark containing 1 item | Spectre.css</title>
	<link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre.min.css">
	<!-- Considered an "experimental" feature -->
	<link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre-exp.min.css" />
	
</head>
<body>
<div class="container">
	
	<div class="timeline">
		<!-- FIRST TICKMARK -->
		<div class="timeline-item">
			<!-- Small circle icon for tickmark -->
			<div class="timeline-left"><a class="timeline-icon" href="#"></a></div><!-- .timeline-left -->
			<div class="timeline-content">
				<!-- TEXT IS CONTAINED IN TILE -->
				<div class="tile">
					<!-- THIS TILE CONTAINS 1 ITEM -->
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

## Example 2: Add items to tickmark

The second example adds another couple of items for that first tickmark. 
They use the class `tile-subtitle`, which by default is the same as `tile-title`.

```html
<!doctype html>
<html lang="en">
<head>
	<!-- Create title for browser tabs & Favorites -->
	<meta charset="utf-8">
	<!-- This site is responsive. Use full screen width. -->
	<link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre.min.css">
	<!-- Considered an "experimental" feature -->
	<link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre-exp.min.css" />
	
</head>
<body>
<div class="container">
	
	<div class="timeline">
		<!-- FIRST TICKMARK -->
		<div class="timeline-item">
			<!-- Small circle icon for tickmark -->
			<div class="timeline-left"><a class="timeline-icon" href="#"></a></div><!-- .timeline-left -->
			<div class="timeline-content">
				<!-- TEXT IS CONTAINED IN TILE -->
				<div class="tile">
					<!-- THIS TILE CONTAINS 3 ITEMS -->
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

File `timeline-minimal-with-subtitle.html` [GitHub Source](https://github.com/tomcam/spectre-book/blob/master/code/timeline-minimal-with-subtitle.html), 
[Preview](https://htmlpreview.github.com/?https://github.com/tomcam/spectre-book/blob/master/code/timeline-minimal-with-subtitle.html)

Example 3: Another tickmark, and tooltip support

```html
<!doctype html>
<html lang="en">
<head>
	<!-- Create title for browser tabs & Favorites -->
	<title>Timeline with 2 tickmarks, tooltip demo | Spectre.css</title>
	<!-- This site is responsive. Use full screen width. -->
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<!-- Ensure use of most common Unicode characters -->
	<meta charset="utf-8">
	<link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre.min.css">
	<!-- Considered an "experimental" feature -->
	<link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre-exp.min.css" />
</head>
<body>
<div class="container">
	
	<div class="timeline">
		
		<!-- FIRST TICKMARK -->
		<div class="timeline-item">
			<!-- Small circle icon for tickmark -->
			<div class="timeline-left"><a class="timeline-icon" href="#"></a></div><!-- .timeline-left -->
			<div class="timeline-content">
				<!-- TEXT IS CONTAINED IN TILE -->
				<div class="tile">
					<!-- THIS TILE CONTAINS 3 ITEMS -->
					<div class="tile-content">
						<p class="tile-title">January</p>
						<p class="tile-subtitle">Get release candidate out</p>
						<p class="tile-subtitle">Update release page</p>
					</div><!-- .tile-content -->
				</div><!-- tile -->
			</div><!-- .timeline-content -->
		</div><!--.timeline -item -->

		<!-- SECOND TICKMARK -->
		<div class="timeline-item">
			<!-- Large circle icon for tickmark -->
			<!-- Add "icon-lg" class to select bigger icon -->
			<!-- Add "tooltip" class for icon's hover-over text -->
			<!-- Text of tooltip comes from "data-tooltip" option -->
			<div class="timeline-left"><a class="timeline-icon icon-lg tooltip" data-tooltip="Oi!" href="#"></a></div><!-- .timeline-left -->
			<div class="timeline-content">
				<!-- TEXT IS CONTAINED IN TILE -->
				<div class="tile">
					<!-- THIS TILE CONTAINS 3 ITEMS -->
					<div class="tile-content">
						<p class="tile-title">February</p>
						<p class="tile-subtitle">First bug pass on release candidate</p>
					</div><!-- .tile-content -->
				</div><!-- tile -->
			</div><!-- .timeline-content -->
		</div><!--.timeline -item -->


	</div><!-- .timeline -->
	
</div><!-- .container -->
</body>
```

File `timeline-second-tickmark.html` [GitHub Source](https://github.com/tomcam/spectre-book/blob/master/code/timeline-second-tickmark.html), 
[Preview](https://htmlpreview.github.com/?https://github.com/tomcam/spectre-book/blob/master/code/timeline-second-tickmark.html)

## Example 4: Add a checked tickmark

Another option for tickmark is a checked version. 
You get this via the `spectre-icons.min.css` style sheet.

Let's add a third, checked tickmark. Just add this `timeline-item`:

```html
<!-- THIRD (CHECKED) TICKMARK -->
<div class="timeline-item">
	<!-- Large circle icon for tickmark -->
	<!-- Add "icon-lg" class to select bigger icon -->
	<div class="timeline-left">
		<a class="timeline-icon icon-lg" href="#">
			<i class="icon icon-check"></i>
		</a>
	</div>
	<div class="timeline-content">
		<!-- TEXT IS CONTAINED IN TILE -->
		<div class="tile">
			<!-- THIS TILE CONTAINS 3 ITEMS -->
			<div class="tile-content">
				<p class="tile-title">Check this, pal</p>
			</div><!-- .tile-content -->
		</div><!-- tile -->
	</div><!-- .timeline-content -->
</div><!--.timeline -item -->
</body>```

The complete file is here:

File `timeline-checked-tickmark.html` [GitHub Source](https://github.com/tomcam/spectre-book/blob/master/code/timeline-checked-tickmark.html), 
[Preview](https://htmlpreview.github.com/?https://github.com/tomcam/spectre-book/blob/master/code/timeline-checked-tickmark.html)


