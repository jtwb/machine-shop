##### Project: Create your own portfolio site on Github Pages

When this project is complete, you will have built a basic portfolio page using HTML and CSS. It will be available at `<your-github-username>.github.io`. It will use Twitter Bootstrap with a custom skin.


## The plan

0. Start with a really basic HTML portfolio page: http://codepen.io/jtwb/pen/ukCyA
0. Customize the content a little
0. Add Twitter Bootstrap to the page
0. Add a Twitter Bootstrap Skin to the page
1. Edit HTML to work with Bootstrap
0. Publish the page on GitHub
0. Customize the page to your liking

## Starting point

(image: basic portfolio page)

## First, open the code in Codepen

(image: codepen code)

Hit the "Fork" button to create your own copy of the project.

You may want to [customize codepen](tech/customize_codepen.md).

## Customize the content a little bit

Try changing the text on the page. Don't worry - you can undo (`⌘ v`) and even re-fork the original project to get back to the start.

Inlcude your name in `<h1>` tag, edit the subtitle, change the `<h2>` sections and link to some cool content you've created. Save your work.

## Add Twitter Bootstrap with a theme

This section requires you to [add a CSS file to your page](tech/add_css_with_a_link_tag.md).

0. Use a `<link>` tag to include `//cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.2.0/css/bootstrap.css` on the page.
0. Use a `<link>` tag to include `//startbootstrap.com/templates/grayscale/css/grayscale.css` on the page.

[More info on no-protocol URLs](http://www.paulirish.com/2010/the-protocol-relative-url/).

(image)

## Make your page match the theme's CSS selectors

Have a look at [the example site for this CSS theme](http://startbootstrap.com/templates/grayscale/). It looks great! So what are we doing wrong?

(image of example site)

The theme CSS file is made up of CSS rules. CSS rules are made of *selectors* and *styles*. We need to write our HTML so that we match those CSS rules.

```css
.brand-heading {
  font-size: 100px;
}
```

To match that CSS rule, we need an element with `class="brand-heading"`.

But that's boring, let's cheat: view the HTML source for the example site.

```html
    <section class="intro">
        <div class="intro-body">
            <div class="container">
                <div class="row">
                    <div class="col-md-8 col-md-offset-2">
                        <h1 class="brand-heading">Grayscale</h1>
                        <p class="intro-text">A free, premium quality, responsive one page Bootstrap theme created by Start Bootstrap.</p>
                        <div class="page-scroll">
                            <a href="#about" class="btn btn-circle">
                                <i class="fa fa-angle-double-down animated"></i>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
```

To get the header section right, you need to edit your HTML so it looks like that.


Looks much better! Here's the updated HTML. I trimmed out some unnecessary elements.

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Me</title>
    <link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.2.0/css/bootstrap.css">
    <link rel="stylesheet" href="http://startbootstrap.com/templates/grayscale/css/grayscale.css">
  </head>
  <body>
    <header class="intro">
      <div class="intro-body">
        <h1 class="brand-heading">I made this</h1>
        <p class="intro-text">In San Francisco, New York and other places</p>
      </div>
    </header>

    <section class="container content-section text-center ui-toolkit">
      <h2>UI toolkit</h2>
      <p><a href="http://github.com">On Github</a><img src="http://f.cl.ly/items/052g1y141x0s1N311c0A/Screen%20Shot%202014-07-11%20at%201.46.13%20PM.png"></p>
    </section>

    <section class="container content-section text-center photography">
      <h2>Graphic art &amp; photography</h2>
      <p><a href="http://www.flickr.com/">Portfolio on Flickr</a></p><img src="http://f.cl.ly/items/040k2P0U1g0U3H391a0c/mona_lisa_polygon_art_by_hand_with_texture__by_trandoductin-d7ff7wd-1.png">
    </section>
  </body>
</html>
```

## Put our images in the background

In the CSS section on CodePen, set the background-image of the `.ui-toolkit` section to point to the URL of [this image](http://f.cl.ly/items/052g1y141x0s1N311c0A/Screen%20Shot%202014-07-11%20at%201.46.13%20PM.png).




#### Techs involved:

* Use Bootstrap CSS
  * Add a CSS file to your page with a Link Tag
* Publish a webpage on GitHub
  * Create a new GitHub repo

###### Tangents:
* Create an HTML page from scratch
* Install git on your machine
