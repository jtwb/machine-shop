#### Tech: Make Codepen.io pretty

**Subject:** http://codepen.io/


## Codepen.io can be pretty

![CodePen screenshot](https://s3.amazonaws.com/machine-shop/Screen+Shot+2014-07-11+at+3.28.06+PM.png)



## Codepen.io can also be ugly

![CodePen screenshot](https://s3.amazonaws.com/machine-shop/Screen+Shot+2014-07-11+at+3.25.19+PM.png)



## Smaller fonts
To adjust the font size just use your browser's "zoom" feature. On OSX you can use `⌘ -`, `⌘ +` and `⌘ 0` to control this. I find that setting the zoom level to ~50% looks pretty good.

## No flickering background
To kill the flickering background, drag this [bookmarklet](http://en.wikipedia.org/wiki/Bookmarklet) to your browser's bookmarks bar. Clicking the bookmark (while you are looking at codepen.io) will kill the flicker problem.

```javascript
javascript:(function(d){var s=d.createElement('style');s.text='.box{background:#252525;}';var h=d.getElementsByTagName('head')[0];h.appendChild(s)})(document);return false;
```
