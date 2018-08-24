# Cards

TODO: Discuss requirement to put it in a grid

Cards display information in panel form, 
presented inside a subtle box outline.
Often they contain an image, a title,
a subtitle, and body text. They can
also contain buttons

## Simple text-only card

A card may contain nothing but text. Normally that would consist of
a title and some sort of body text. Technically

The minimum card is wrapped inside a div of class `card`.
It normally has a `header` div nested inside it, and
within the `header` div is a `card-title` div.

Following that is a div of class `card-body`. Here's an abbreviated example:

```html
<div class="card">
        <div class="card-header">
          <div class="card-title h4">
            Title
          </div><!-- .card-title -->    
        </div><!--- .card-header -->
        <div class="card-body">
            Body text
        </div><!-- .card-body --> 
</div><!-- .card -->

```


```html
<!doctype html>                                                                                                                                          
<html lang="en">                                                             
<head>                                                                     
                       
        <!-- Create title for browser tabs & Favorites -->                                                     
        <title>Text-only card example | Spectre.css</title>                     
        <!-- This site is responsive. Use full screen width. -->                
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <!-- Ensure use of most common Unicode characters -->
        <meta charset="utf-8">
        <link rel="stylesheet" href="https://unpkg.com/spectre.css/dist/spectre.min.css">
<style> 
         
</style>           
</head>                                
<body>         
        <div class="container"> 
                <div class="columns">
                        <div class="column col-4">
                             
                                <div class="card">
                                        <div class="card-header">
                                                <div class="card-title h4">
                                                        Classic CSS text updated
                                                </div><!-- .card-title -->    
                                        </div><!--- .card-header -->
                                        <div class="card-body">
                                                A classic and surprisingly affordable
                                                text on efficient CSS has been updated
                                                due to popular demand.
                                        
                                                "The Least You Need to Know About Spectre.css" book 
                                                from EasyOnMe Press was released to almost
                                                unanimous acclaim two years ago. It has
                                                been updated to reflect changing times
                                                and profligate use of CPU cycles.
                                  
                                                <a href="#"><span class="text-success">MORE</a>
                                  
                                        </div><!-- .card-body --> 
                                </div><!-- .card -->
                     
                        </div>
                </div>
        </div><!-- .container -->
</body>                      
~

```


## Simple card with image

