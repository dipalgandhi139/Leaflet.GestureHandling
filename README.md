# Leaflet.GestureHandling

Prevents users from getting trapped on the map when scrolling a long page. 

Brings the basic functionality of [Google Maps Gesture Handling](https://developers.google.com/maps/documentation/javascript/examples/interaction-cooperative) into Leaflet.

**On Desktop**

![alt text](https://elmarquis.github.io/Leaflet.GestureHandling/examples/images/desktop.png "Desktop")

- The map ignores the mouse scroll wheel.
- The user is prompted to use ctrl+scroll to zoom the map. 

**On Mobile / Touch devices**

![alt text](https://elmarquis.github.io/Leaflet.GestureHandling/examples/images/mobile.png "Mobile")

- The map ignores single fingered dragging. 
- The user is prompted to use two fingers to pan the map. 


## Demo
[View demo](https://elmarquis.github.io/Leaflet.GestureHandling/examples/)

## Install
The latest leaflet-gesture-handling can be downloaded from the dist folder. 

## Usage
Include the css and js file after leaflet.js. 
```
<link rel="stylesheet" href="css/leaflet-gesture-handling.css" type="text/css">
<script src="js/leaflet-gesture-handling.js"></script>
```

Set **gestureHandling: true** in your map initialization script. 

```
 var map = L.map("map", {
    center: [-25.2702, 134.2798],
    zoom: 3,
    gestureHandling: true
});
```

## Useful info
GestureHandling disables the following map attributes. 
- dragging
- tap
- scrollWheelZoom

They are temporarily enabled for the duration the user scrolls with ctrl+mousewheel or uses two fingers to pan the map on mobile. 

## Compatibility with other plugins
I have added compatibility with [Leaflet-MiniMap](https://github.com/Norkart/Leaflet-MiniMap). It allows the user to still pan around the minimap with a single finger.

If there's any other plugins you'd like this to work with, let me know or submit a pull request. 

## License
MIT

