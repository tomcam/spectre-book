<link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre.min.css">
<link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre-icons.min.css">

# Using the Spectre.css built-in CSS icon set

Spectre.css has a small but well-chosen set of CSS-only [icons](https://github.com/picturepan2/spectre/blob/master/dist/spectre-icons.css)
Because they're pure CSS they contribute little
to page size, keeping your web pages lean and fast. 
As is the custom with many other style sheet frameworks,
the italics `<i>` tag is abused for this purpose. 
Using the italics tag to produce italicized text is now frowned upon because it's not semantic.
Modern developers are expected to use the `<em>` tag instead of `<i>`. This frees up the fortuitously named `<i>` for icons. 


## How to specify an icon

1. Remember to include the `spectre-icons.min.css` (or `spectre-icons.css`) style sheet.
2. Use icons as you would text. All icons are wrapped inside an `<i>` tag and must include 
two classes: `icon` (which defines the physical properties common to all Spectre
icons) and the class name of the icon itself, for example, `icon-time` for 
the clock icon.

The simplest possible case looks like this:

```html
<i class="icon icon-time"></i>
```

Or, in full context:

```html{8-9,12}
<!doctype html>
<html lang="en">
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Icon test | Spectre.css</title>
	<link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre.min.css">
	<!-- Use Spectre's pure CSS icons -->
	<link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre-icons.min.css"> 
</head>
<body>
    <i class="icon icon-time"></i>
</body>
```
File `min-icon.html` [GitHub Source](https://github.com/tomcam/spectre-book/blob/master/examples/min-icon.html), 
[Preview](https://htmlpreview.github.com/?https://github.com/tomcam/spectre-book/blob/master/examples/min-icon.html)


<p>The above code produces this result:</p>
<i class="icon icon-time"></i>

## Creating icons in 2x, 3x, or 4x sizes

Specify a size of 2x, 3x, or 4x to make it bigger:

```html
<i class="icon icon-2x icon-time"></i>
<i class="icon icon-3x icon-time"></i>
<i class="icon icon-4x icon-time"></i>
```
 
The result:

<i class="icon icon-2x icon-time"></i>
<i class="icon icon-3x icon-time"></i>
<i class="icon icon-4x icon-time"></i>

## List of all Spectre.css icons

| Icon                                                | Description               | Spectre.css Markdown |
| --------------------------------------------------- | ------------------------- | -------------------- |      
| <i class="icon icon-2x icon-time"></i>              | Clock                     | icon-time            |
| <i class="icon icon-2x icon-people"></i>            | Person                    | icon-people          |
| <i class="icon-flag icon icon-2x"></i>              | Flag                      | icon-flag            |                                                                                                  
| <i class="icon-arrow-down icon icon-2x"></i>        | Caret pointing down       | icon-arrow-down      |                                                                                                
| <i class="icon-arrow-up icon icon-2x"></i>          | Caret pointing up         | icon-arrow-up        |                                                                                              
| <i class="icon-arrow-left icon icon-2x"></i>        | Caret pointing left       | icon-arrow-left      |                                                                                                  
| <i class="icon-arrow-right icon icon-2x"></i>       | Caret pointing right      | icon-arrow-right     |                                                                                                     
| <i class="icon-downward icon icon-2x"></i>    | Arrow pointing down       | icon-downward  |                                                                                                 
| <i class="icon-upward icon icon-2x"></i>      | Arrow pointing up         | icon-upward    |                                                                                                  
| <i class="icon-back icon icon-2x"></i>              | Arrow pointing left       | icon-back            |                                                                                                       
| <i class="icon-forward icon icon-2x"></i>           | Arrow pointing right      | icon-forward         |                                                                                                        
| <i class="icon-caret icon icon-2x"></i>             | Solid caret pointing down | icon-caret           |                                                                                                           
| <i class="icon-menu icon icon-2x"></i>              | Hamburger Menu            | icon-menu            |                                                                                                            
| <i class="icon-apps icon icon-2x"></i>              | Applications              | icon-apps            |                                                                                                            
| <i class="icon-resize-horiz icon icon-2x"></i>      | Resize horizontally       | icon-resize-horiz    |                                                                                              
| <i class="icon-resize-vert icon icon-2x"></i>       | Resize vertically         | icon-resize-vert     |                                                                                                     
| <i class="icon-more-horiz icon icon-2x"></i>        | Horizontal indicator      | icon-more-horiz      |                                                                                                      
| <i class="icon-more-vert icon icon-2x"></i>         | Vertical indicator        | icon-more-vert       |                                                                                                       
| <i class="icon-plus icon icon-2x"></i>              | Plus                      | icon-plus            |                                                                                                           
| <i class="icon-minus icon icon-2x"></i>             | Minus                     | icon-minus           |                                                                                                          
| <i class="icon-check icon icon-2x"></i>             | Checkmark                 | icon-check           |                                                                                                          
| <i class="icon-cross icon icon-2x"></i>             | Cross/uncheck             | icon-cross           |                                                                                                          
| <i class="icon-stop icon icon-2x"></i>              | Stop/prohbited            | icon-stop            |                                                                                                          
| <i class="icon-shutdown icon icon-2x"></i>          | Shutdown/power off        | icon-shutdown        |                                                                                               
| <i class="icon-refresh icon icon-2x"></i>           | Refresh                   | icon-refresh         |                                                                                                                
| <i class="icon-search icon icon-2x"></i>            | Search/magnifying glass   | icon-search          |                                                                                                          
| <i class="icon-edit icon icon-2x"></i>              | Edit                      | icon-edit            |                                                                                                            
| <i class=" icon-delete icon icon-2x"></i>           | Delete                    | icon-delete          |                                                                                                          
| <i class="icon-share icon icon-2x"></i>             | Share                     | icon-share           |                                                                                                        
| <i class="icon-flag icon icon-2x"></i>              | Flag                      | icon-flag            |                                                                                                          
| <i class="icon-bookmark icon icon-2x"></i>          | Bookmark                  | icon-bookmark        |                                                                                                       
| <i class="icon-download icon icon-2x"></i>          | Download                  | icon-download        |                                                                                                    
| <i class="icon-upload icon icon-2x"></i>            | Upload                    | icon-upload          |                                                                                                   
| <i class="icon-mail icon icon-2x"></i>              | Mail                      | icon-mail            |                                                                                                           
| <i class="icon-message icon icon-2x"></i>           | Message                   | icon-message         |                                                                                                    
| <i class="icon-photo icon icon-2x"></i>             | Camera                    | icon-photo           |                                                                                                       
| <i class="icon-link icon icon-2x"></i>              | Link                      | icon-link            |                                                                                                          
| <i class=" icon-location icon icon-2x"></i>          | Location (map pin)        | icon-location        |                                                                                                     
| <i class="icon-emoji icon icon-2x"></i>             | Emoji                     | icon-emoji           |                

## Reference

Source code for all [Spectre.css icons](https://github.com/picturepan2/spectre/blob/master/dist/spectre-icons.css)

