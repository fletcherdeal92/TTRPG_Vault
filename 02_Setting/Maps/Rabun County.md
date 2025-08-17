---
map_height_y: 2550
map_width_x: 3300
scale_pixels: 800
scale_pixels_range: 6
mapCalc1: 0.0075
---

> [!NOTE]- Quick Calculator  
> Map Height in Pixels: `INPUT[number:map_height_y]`  
> Map Width in Pixels: `INPUT[number:map_width_x]`  
> lat: `VIEW[{map_height_y} / 2][math]`  
> long: `VIEW[{map_width_x} / 2][math]`  
> How Many Pixels In Scale: `INPUT[number:scale_pixels]`  
> How Many Units in Scale: `INPUT[number:scale_pixels_range]`  
> Scale: `VIEW[1/({scale_pixels}/{scale_pixels_range})][math:mapCalc1]`



```leaflet  
id: RabunCounty ### Must be unique with no spaces  
image: [[Rabun_Map_NewRail_Labeled.png]] ### Link to the map image file. Do not add a ! in front of the image  
bounds: [[0,0], [3300, 2550]] ### Size of the map in px Height_y, Width_x. Ignore 0,0  
height: 850px ### Size of the leaflet embed in px on your screen  
width: 100% ### Size of the leaflet embed in your note  
lat: 1100 ### To center the map, make this half of the map height.  
long: 625 ### To center the map, make this half of the map width.  
minZoom: -2 ### Controls how far away from the map you can zoom out. Hover over the target icon to see the current level.  
maxZoom: 2 ### Controls how far towards the map you can zoom in. Hover over the target icon to see the current level.  
defaultZoom: .25 ### Sets the default zoom level when the map loads. Hover over the target icon to see the current level.  
zoomDelta: 0.25 ### Adjust how much the zoom changes when you zoom in or out.  
unit: mi ### The value displayed when measuring so you know what type of unit is being measure.  
scale: 0.0075 ### Real units/px (resolution) of your map  
recenter: false  
darkmode: false ### markermarker: default,1099.4720629442318,614.2748313428385,Tallulah Falls,,,

```
