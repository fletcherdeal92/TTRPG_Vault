---
type: location
created: 2025-08-11
updated: 2025-08-11
tags:
  - location
region: Northeast Georgia Mountains
settlement_type: transport
danger_level: safe
population: 40
primary_industry: none
old_gods_influence: minor
---

# Train_Car

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

## Notable NPCs
```dataview
TABLE without id file.link as "Name", faction as "Faction", trust_level as "Trust"
FROM #npc
WHERE location = this.file.name
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
WHERE contains(locations_visited, this.file.name)
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
