# Notes on how CSS is used by Spectre.css


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

The `rem` unit is based on the height of the default font, which is an attribute of the `<html>` 
element. (Technically it is based on what the CSS specification terms the "root element," which
could in theory be another medium such as print. We'll use the term default font here for clarity.) 
So if you see something like this, you know that the `<h1>` tag height will be 60 pixels:

```css
html { font-size: 20px; }
h1   { font-size: 3em; }    /* Computes to 60px */
```

## em is based on the calculated font size

The `em` unit is based on the height of the current HTML element, which is calculated
based on the current element.

The following example is extracted from Spectre.css: 

```css
/* Based on Spectre.css */
html { font-size: 20px; }
h1 { font-size: 2em; }          /* Computes to 40px */
h2 { font-size: 1.6rem; }       /* Computes to 32px */
h1, h2 { margin-bottom: .5em; } /* So h1 = 20px, h2 = 16 px */
```

As you can see, the `margin-bottom` attribute of the `<h1>` and `<h2>` tags is derived from the sizes of
the elements themselves, not the html root. 

Because the `html` attribute's font size has been set to 20 pixels, each `em` means 20 pixels. So: 

* An `<h1>`font is therefore 40 pixels high, and `.5em` means half the computed height of the current font, or 20 pixels. Therefore the `<h1>` bottom margin is 20 pixels. 
* An `<h2>` is 32 pixels high. Its height is computed as 1.6 multiplied by the 20 pixel base font height. Its bottom margin of `.5em` means half of that computed height, or 16 pixels.

Suppose the `margin-bottom` were specified in `rem` units instead. In that case the computation would be simple,
because it's the same for both: `.5rem` means half the height of the default font (not the computed height of the current font, in this case the
`<h1>` or `<h2>` tag).

```css
/* Different from Spectre.css */
html { font-size: 20px; }
h1 { font-size: 2em; }           /* Computes to 40px */
h2 { font-size: 1.6rem; }        /* Computes to 32px */
h1, h2 { margin-bottom: .5rem; } /* Computes to 20px for both */
```



