# Google Maps Tutorial
---
This tutorial shows you how to add a simple Google map to a web page. It suits people with beginner or intermediate knowledge of HTML and CSS, and a little knowledge of JavaScript. For an advanced guide to creating maps, read the [Google Maps Javascript API developer's guide](https://developers.google.com/maps/documentation/javascript/tutorial).
---
### 1. Create an HTML page

Create a html containing simple html with a `div` for holding the map. We give that `div` id of `map`. We also specify width, height and background color for `#map` element.

```html
<!DOCTYPE html>
<html>
  <head>
    <style>
      #map {
        width: 100%;
        height: 400px;
        background-color: grey;
      }
    </style>
  </head>
  <body>
    <h3>Purdue Ironhacks Google Maps Tutorial</h3>
    <div id="map"></div>
  </body>
</html>
```
