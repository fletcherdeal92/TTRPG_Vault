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
---

# Tallulah Falls

![[Town of tallulah falls_labeled_northArrow.png]]

## Description
- **Physical layout:** 
- **Atmosphere:** 
- **Notable features:** 
- **Local folklore:** 

## History & Background
- **Founded/discovered:** European settlers named it c. 1820, incorporated October 7, 1885
- **Key events:** 
  - 1882: Tallulah Falls Railroad arrives
  - 1885: Town incorporated, R.L. Moss Sr. founding commissioner
  - 1913: Tallulah Falls Dam completed, waterfalls reduced to trickle
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
