##### Tech: Adding a new CSS file to a page using a `<link>` tag

This is the standard way to add a CSS file to an HTML page.

When someone opens your HTML page, their browser will download all the files it finds in `<link>` tags on the page before displaying the page to the user.

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Page title</title>
    <link rel="stylesheet" href="/my-styles.css">
  </head>
  <body>
    
    <header>
      <h1>I made this</h1>
      <p>In San Francisco, New York and other places</p>
    </header>
    
    <section>
      <h2>UI toolkit</h2>
      <p><a href="http://github.com">On Github</a><img src="http://f.cl.ly/items/052g1y141x0s1N311c0A/Screen%20Shot%202014-07-11%20at%201.46.13%20PM.png"></p>
    </section>
      
    <section>
      <h2>Graphic art &amp; photography</h2>
      <p><a href="http://www.flickr.com/">Portfolio on Flickr</a></p><img src="http://f.cl.ly/items/040k2P0U1g0U3H391a0c/mona_lisa_polygon_art_by_hand_with_texture__by_trandoductin-d7ff7wd-1.png">
    </section>
  </body>
</html>
```

##### Here's what the parts of the link tag mean:

## HREF

```html
href="/my-styles.css"
```
A URL of a CSS file.

## REL

```html
rel="stylesheet"
```

Designates your file as a stylesheet. This tells the browser to apply the rules in your CSS file to elements on the page.

If you omit or change `rel`, the browser may not apply your CSS rules to the page. For example, this would tell the browser to download `/styles-for-page-2.css` without reading its contents, so that if you visit `/page-2.html` you will already have the CSS for that page.
```html
<link rel="prefetch" href="/styles-for-page-2.css">
```
