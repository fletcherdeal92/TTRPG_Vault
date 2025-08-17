---
type: location
created: 2025-08-11
updated: 2025-08-11
tags:
  - location
location_type: 
parent_location: "[[]]"
region: Northeast Georgia Mountains
settlement_type: town
danger_level: safe
population: 2000
primary_industry: hospitality
old_gods_influence: minor
artifacts_found: 
special_rules: 
map_height_y: 2048
map_width_x: 1642
scale_pixels: 268
scale_pixels_range: 24
mapCalc1: 0.08955223880597016
---

# Tallulah Falls
![[Tallulah_Falls_Painting_Town.jpg]]
*Tallulah Falls, before the boom*
## Description
- **Physical layout:** 
- **Atmosphere:** 
- **Notable features:** 
- **Local folklore:** 

## History & Background
- **Founded/discovered:** European settlers named it c. 1820, incorporated October 7, 1885
- **Key events:** 
  - *1882:* Tallulah Falls Railroad arrives
  - *1885:* Town incorporated, R.L. Moss Sr. founding commissioner
  - *1913:* Tallulah Falls Dam completed, waterfalls reduced to trickle
- **Old Gods influence:** Cherokee called the falls "Ugunyi" and avoided the area

## Current Situation (1920s)
- **Population:** ~2000 peak season, ~500 year-round
- **Primary industry:** Tourism via railroad from Atlanta
- **Leadership:** 
- **Tensions/conflicts:** 

## Supernatural Elements
- **Strange occurrences:** 
- **Local legends:** 
- **Warning signs:** 

## Map

```leaflet  
id: TallulahFalls ### Must be unique with no spaces  
image: [[Town of tallulah falls_labeled_northArrow.png]] ### Link to the map image file. Do not add a ! in front of the image  
bounds: [[0,0], [1500, 2000]] ### Size of the map in px Height_y, Width_x. Ignore 0,0  
height: 850px ### Size of the leaflet embed in px on your screen  
width: 95% ### Size of the leaflet embed in your note  
lat: 1024 ### To center the map, make this half of the map height.  
long: 1020 ### To center the map, make this half of the map width.  
minZoom: -1.5 ### Controls how far away from the map you can zoom out. Hover over the target icon to see the current level.  
maxZoom: 1 ### Controls how far towards the map you can zoom in. Hover over the target icon to see the current level.  
defaultZoom: -1 ### Sets the default zoom level when the map loads. Hover over the target icon to see the current level.  
zoomDelta: 0.5 ### Adjust how much the zoom changes when you zoom in or out.  
unit: mi ### The value displayed when measuring so you know what type of unit is being measure.  
scale: 0.09328358208955223 ### Real units/px (resolution) of your map  
recenter: false  
darkmode: false ### marker
```




## NPCs Present Here
```dataview
TABLE without id file.link as "Name", faction as "Faction", trust_level as "Trust"
FROM #npc
WHERE current_location = "[[" + this.file.name + "]]"
```

## NPCs From Here
```dataview
TABLE without id file.link as "Name", faction as "Faction", current_location as "Currently At"
FROM #npc
WHERE home_location = "[[" + this.file.name + "]]"
```

## NPCs Who Visit Here
```dataview
TABLE without id file.link as "Name", faction as "Faction", trust_level as "Trust"
FROM #npc
WHERE contains(notable_locations, "[[" + this.file.name + "]]")
```

## Artifacts & Items Found Here
```dataview
TABLE without id file.link as "Item", type as "Type", danger_level as "Danger"
FROM #artifact
WHERE current_location = this.file.name
```

## Session History
```dataview
TABLE without id file.link as "Session", date as "Date", summary as "What Happened"
FROM #session
WHERE contains(locations_visited, "[[" + this.file.name + "]]")
```

## Connected Locations
- **Roads/paths to:** 
- **Travel time:** 4 hours by train from Atlanta
- **Travel dangers:** 

## Adventure Hooks
- 
- 
- 

## GM Notes
**Secrets:**
- 

**Foreshadowing:**
- 

**Environmental Hazards:**
- 
