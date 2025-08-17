---
type: location
created: 2025-08-13
updated: 2025-08-13
tags:
  - location
location_type: area
parent_location: "[[Cliff House]]"
region: Tallulah Falls
settlement_type: none
danger_level: caution
population: 
primary_industry: 
old_gods_influence: 
artifacts_found: 
special_rules:
---

# Cliff House - Overlook

Leaving the Cliff House, if you look to the left (northish) along the front porch you would notice a well worn path to the open overlook of the gorge that the cliff house affords. If you look straight down you could just make out the far edge of what the locals call Hawthorne's Pool. Looking left you could just make out parts of the majestic L'Eau'D'or falls as it tumbles into the pool. Look left and you can see the water crest over hurricane falls. A path starts down the gorge, it is rugged, but pains have been made to take care of it and there seems to be some parts with wooden stairs. a sign to it's right say's Trail to Observation Tower

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
