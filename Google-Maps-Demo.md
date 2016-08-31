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
    <script type="text/javascript">
	function initMap(){
		var mapDiv = document.getElementById('map');
		var map = new google.maps.Map(mapDiv, {
			center: {lat: 40.4237, lng: 86.9212},
			zoom: 16});
		var marker = new google.maps.Marker({ //Line 1
			position: {lat: 40.4237, lng: 86.9212}, //Line2: Location to be highlighted
			map: map,//Line 3: Reference to map object
			title: 'Purdue University' //Line 4: Title to be given
		})
	}
	</script>
  </head>
  <body>
    <h3>Purdue Ironhacks Google Maps Tutorial</h3>
    <div id="map"></div>
  </body>
  <script async defer
	src="https://maps.googleapis.com/maps/api/js?key=AIzaSyCC4lO1PjOC9xzRaOK86FJoht6VBFYcsB8&callback=initMap">
</script>
</html>