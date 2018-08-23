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

## Example 2

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
