#### Tech: Make Codepen.io pretty

**Subject:** http://codepen.io/


## Codepen.io can be pretty

<p align="center">
<img src="https://s3.amazonaws.com/machine-shop/Screen+Shot+2014-07-11+at+3.28.06+PM.png" alt="CodePen screenshot" width="570"/>
</p>


## Codepen.io can also be ugly

<p align="center">
<img src="https://s3.amazonaws.com/machine-shop/Screen+Shot+2014-07-11+at+3.25.19+PM.png" alt="CodePen screenshot" width="570"/>
</p>


## Smaller fonts
To adjust the font size just use your browser's "zoom" feature. On OSX you can use `⌘ -`, `⌘ +` and `⌘ 0` to control this. I find that setting the zoom level to ~50% looks pretty good.

## No flickering background
To kill the flickering background, drag this [bookmarklet](http://en.wikipedia.org/wiki/Bookmarklet) to your browser's bookmarks bar. Clicking the bookmark (while you are looking at codepen.io) will kill the flicker problem.

```javascript
javascript:(function(d){var s=d.createElement('style');var h=d.getElementsByTagName('head')[0];s.innerHTML='.box{background:#252525 !important;}';h.appendChild(s)})(document);
```

Select that text and drag it to your bookmarklets bar. You may want to rename the bookmarklet to something like "Fix codepen".

Alternatively you can create a new bookmark and paste that code where the URL would go.
