---
type: location
created: 2025-08-11
updated: 2025-08-11
tags:
  - location
location_type: transportation
parent_location: "[[]]"
region: Tallulah Falls
settlement_type: none
danger_level: safe
population: 0
primary_industry: none
old_gods_influence: minor
artifacts_found: []
special_rules: []
---

# Train Car

<% tp.file.cursor(1) %>

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
