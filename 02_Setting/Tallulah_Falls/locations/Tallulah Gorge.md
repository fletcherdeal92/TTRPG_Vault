---
type: location
created: 2025-08-11
updated: 2025-08-11
tags: [location]
region: Northeast Georgia Mountains
settlement_type: wilderness
danger_level: 
population: 0
primary_industry: 
old_gods_influence: 
---

# Tallulah Gorge

## Description
- **Physical layout:** 
- **Atmosphere:** 
- **Notable features:** 
- **Local folklore:** 

## History & Background
- **Founded/discovered:** 2 miles long, nearly 1,000 feet deep canyon carved by Tallulah River
- **Key events:** 
  - Pre-1820: Cherokee name "Ugunyi", avoided the area
  - 1842: Thomas Addison Richards' engravings in Georgia Illustrated popularized nationally
  - 1913: Dam diverted river through 6,666-foot tunnel, waterfalls reduced to trickle
- **Old Gods influence:** Six major waterfalls: L'Eau d'Or (46ft), Tempesta (81ft), Hurricane (96ft), Oceana (42ft), Bridal Veil Falls, plus sixth unnamed

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