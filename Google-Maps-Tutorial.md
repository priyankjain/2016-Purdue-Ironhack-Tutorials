# Google Maps Tutorial
   
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

### 2. Get an API key

   Follow these steps to get an API key
   1. Go to the [Google API Console](https://console.developers.google.com/flows/enableapi?apiid=maps_backend,geocoding_backend,directions_backend,distance_matrix_backend,elevation_backend,places_backend&keyType=CLIENT_SIDE&reusekey=true).
   2. Create or select a project.
   3. Click continue to enable the API and any related services.
   4. On the Credentials page, get a Browser key.
   5. Save the API key you get in a browser window. We would call it **_YOUR_API_KEY_** for rest of the tutorial

### 3. Load Google Maps Scripts

To load google maps in your webpage, include the following script tag in your webpage.

```html
<script async defer
src="https://maps.googleapis.com/maps/api/js?key=**YOUR_API_KEY**&callback=initMap">
</script>
```
Replace YOUR_API_KEY with your API key obtained from step 2.
