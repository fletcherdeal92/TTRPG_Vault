---
type: location
created: 2025-08-17
updated: 2025-08-17
tags:
  - location
location_type: area
parent_location: "[[Tallulah Falls]]"
region: Northeast Georgia Mountains
settlement_type: none
danger_level: caution
population: 
primary_industry: 
old_gods_influence: 
artifacts_found: 
special_rules:
---

# Tallulah Gorge
![[Tallulah_Falls_Painting.jpg]]



## Description
- **Physical layout:** 
- **Atmosphere:** 
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
