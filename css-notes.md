# Notes on how CSS is used in this book


## The default html font size is not guaranteed

If no style sheet is specified, your browser has a default font size 
for the `html` element. It's usually 16 pixels, but there are
no guarantees in any Web specifications, which makes sense because
most browsers let you change the pixel size of the default font. 
That's why one of the first things any CSS framework
does is establish some kind of default font size. Spectre.css sets it to 20 pixels.
(If 20px seems too large, you'll find that readability studies show it to be the
best compromise for the largest audience.)

In the bad old days, designers would specify font sizes using pixels, like
this:

```css
h1 { font-size: 60px; } /* Ugh! Not very scalable */
```

Using pixels for CSS elements makes zooming and resizing of fonts less predictable. 
Also, many CSS designs are based on the font size, so a relative unit size makes
the designs far more flexible.

## rem is the same as the html font size

The `rem` unit is based on the height of the default browser font, which is an attribute of the `html` 
element. So if you see something like this, you know that the `h1` height will be 60 pixels:

```css
html { font-size: 20px; }
h1   { font-size: 3em; }    /* Computes to 60px */
```

##



Spectre.css normally `rem` and `em` to size elements, in place of hardcoded pixel sizes. 
This makes it easy to adjust font sizes 
using your browser. It also makes accessibility easier for sight-impaired users.

### `em` is based on your browser's default font size

The `em` unit is relative. It inherits your browser's default font size. 
Most browsers default to a font size 16 pixels high, expressed as `16px` in a style sheet. 
Therefore on most browsers if you declared that an `h1` element used a `font-size` of `3em` 
it would be 48 pixels high.



