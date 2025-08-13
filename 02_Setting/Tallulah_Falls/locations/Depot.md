---
type: location
created: 2025-08-12
updated: 2025-08-12
tags:
  - location
location_type: building
parent_location: "[[Tallulah Falls]]"
region: Tallulah Falls
settlement_type: none
danger_level: safe
population: 
primary_industry: 
old_gods_influence: 
artifacts_found: 
special_rules:
---

# Depot

The Tallulah falls depot is; in a word, unimpressive, for the resort town that it serves. Its pine wooden walls rise up to meet the roof at a sharp angle. the roof overhangs the wooden platform with dark arched beams coming from the station. 

## Description
- **Physical layout:** When looking at the station as you step off a north-bound train you notice to the left a window where the clerk office sits behind. You could speak to him to get a ticket further up the line to Clayton, or send off an urgent wire. To the right, under the second story gabled window, a large open door faces into the storage room for the depot various large boxes and parcels await for destinations unknown. If you were to walk left and turn the corner, you'd find a short set of stairs leading on to the "platform" though the tracks were feet away from it, negating it's usefulness. Through the door across those steps you would find a door that leads into the station's modest sitting room.
- **Atmosphere:** In this cool, northeast Georgian, summer day the station feels like warmth and nostalgia. I+n across from the Cliff House makes the station even more lively with the 50 piece cliff house band  
- **Notable features:** 
- **Local folklore:** 

## History & Background
- **Founded/discovered:** 
- **Key events:** 
- **Old Gods influence:** 

## Current Situation (1920s)
- **Population:** 
- **Primary industry:** 
- **Leadership:** 
- **Tensions/conflicts:** 

## Supernatural Elements
- **Strange occurrences:** 
- **Local legends:** 
- **Warning signs:** 

## NPCs Present Here
```dataview
TABLE without id file.link as "Name", faction as "Faction", trust_level as "Trust"
FROM #npc
WHERE current_location = link(this.file.name)
```

## NPCs From Here
```dataview
TABLE without id file.link as "Name", faction as "Faction", current_location as "Currently At"
FROM #npc
WHERE home_location = link(this.file.name)
```

## NPCs Who Visit Here
```dataview
TABLE without id file.link as "Name", faction as "Faction", trust_level as "Trust"
FROM #npc
WHERE contains(notable_locations, link(this.file.name))
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
- **Travel time:** 
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
