# Campaign Dashboard - Written in Water

*Master overview of all campaign elements with dynamic dataview queries*

## Campaign Overview
**Current Adventure:** The Path Below (Adventure 1)  
**Setting:** Tallulah Falls, Georgia - Fall 1923  
**Campaign Theme:** Old Gods of Appalachia cosmic horror  

## Quick Navigation
- [[#Session Tracker]]
- [[#Character Relationships]]
- [[#Location Status]]
- [[#Artifact Inventory]]
- [[#Rules Reference]]
- [[#Faction Overview]]

---

## Session Tracker
### Recent Sessions
```dataview
TABLE WITHOUT ID 
  file.link as "Session",
  session_number as "#",
  date as "Date",
  duration + " hrs" as "Length",
  players_present as "Players"
FROM #session
SORT session_number DESC
LIMIT 5
```

### Session Timeline
```dataview
TABLE WITHOUT ID
  session_number as "#",
  file.link as "Session",
  locations_visited as "Locations",
  npcs_encountered as "NPCs Met",
  artifacts_discovered as "Items Found"
FROM #session
SORT session_number ASC
```

---

## Character Relationships
### All NPCs by Trust Level
```dataview
TABLE WITHOUT ID
  file.link as "NPC",
  location as "Location",
  faction as "Faction",
  trust_level as "Trust",
  character_type as "Type",
  status as "Status"
FROM #npc
SORT trust_level ASC, file.name ASC
```

### NPCs by Location
```dataview
TABLE WITHOUT ID
  location as "Location",
  file.link as "NPC",
  trust_level as "Trust",
  knowledge_level as "Awareness"
FROM #npc
SORT location ASC, trust_level ASC
```

---

## Location Status
### All Locations
```dataview
TABLE WITHOUT ID
  file.link as "Location",
  region as "Region",
  danger_level as "Danger",
  old_gods_influence as "OG Influence",
  population as "Population"
FROM #location
SORT danger_level DESC, old_gods_influence DESC
```

### Supernatural Hotspots
```dataview
TABLE WITHOUT ID
  file.link as "Location",
  old_gods_influence as "Influence Level",
  danger_level as "Danger",
  settlement_type as "Type"
FROM #location
WHERE old_gods_influence = "strong" OR old_gods_influence = "moderate" OR old_gods_influence = "overwhelming"
SORT old_gods_influence DESC
```

---

## Artifact Inventory
### All Artifacts
```dataview
TABLE WITHOUT ID
  file.link as "Item",
  category as "Category",
  danger_level as "Danger",
  current_location as "Location",
  current_owner as "Owner"
FROM #artifact
SORT danger_level DESC, category ASC
```

### Supernatural Items
```dataview
TABLE WITHOUT ID
  file.link as "Item",
  old_gods_connection as "OG Connection",
  current_location as "Location",
  discovery_session as "Found In"
FROM #artifact
WHERE old_gods_connection != "none" AND old_gods_connection != null
SORT old_gods_connection DESC
```

---

## Rules Reference
### House Rules Quick Reference
```dataview
TABLE WITHOUT ID
  file.link as "Rule",
  category as "Type",
  complexity as "Complexity",
  frequency as "Usage"
FROM #rule
SORT frequency ASC, complexity ASC
```

### Supernatural Rules
```dataview
TABLE WITHOUT ID
  file.link as "Rule",
  applies_to as "Applies To",
  complexity as "Complexity"
FROM #rule
WHERE category = "supernatural" OR applies_to = "supernatural"
SORT complexity ASC
```

---

## Investigation Tracker
### Current Mysteries
- **Professor Whitaker's Disappearance**: Missing for 3 days from Cliff House
- **Panther Creek Phenomena**: Geological anomalies and supernatural activity
- **Local Warning Patterns**: Why locals avoid certain areas

### Evidence Collected
```dataview
TABLE WITHOUT ID
  file.link as "Evidence",
  discovery_session as "Session Found",
  current_location as "Currently At"
FROM #artifact
WHERE discovery_session != null
SORT discovery_session ASC
```

### Key Witnesses
```dataview
TABLE WITHOUT ID
  file.link as "NPC",
  knowledge_level as "What They Know",
  trust_level as "Willingness to Share"
FROM #npc
WHERE knowledge_level = "aware" OR knowledge_level = "involved" OR knowledge_level = "suspicious"
SORT knowledge_level DESC, trust_level DESC
```

---

## Danger Assessment
### Threat Levels by Location
```dataview
TABLE WITHOUT ID
  file.link as "Location",
  danger_level as "Physical Danger",
  old_gods_influence as "Supernatural Danger",
  population as "Witnesses Present"
FROM #location
SORT danger_level DESC, old_gods_influence DESC
```

### Hostile or Dangerous NPCs
```dataview
TABLE WITHOUT ID
  file.link as "NPC",
  location as "Location",
  trust_level as "Attitude",
  status as "Current Status"
FROM #npc
WHERE trust_level = "hostile" OR trust_level = "wary" OR status = "missing" OR status = "transformed"
```

---

## Campaign Progress
### Adventure Arc Status
- **The Path Below**: Investigation phase - characters gathering information about Whitaker's disappearance
- **Next Steps**: Likely investigation of Panther Creek based on research notes
- **Long-term**: Understanding the true nature of Old Gods influence in the region

### Character Development Opportunities
- Building trust with local community members
- Learning protective folklore and rituals
- Understanding the balance between investigation and safety

---

## GM Notes Section
*Quick references for session prep*

### Immediate Plot Threads
1. **Whitaker's Fate**: Players need to decide whether to investigate Panther Creek
2. **Local Relationships**: Building trust with Elmer and Martha Hutchins
3. **Supernatural Evidence**: Strange Geological Samples providing detection capability

### Upcoming Encounters
- **Panther Creek Investigation**: High danger, major supernatural encounter likely
- **Cherokee Elder Contact**: Potential source of protective knowledge
- **Eleanor Thorne Confrontation**: Hotel proprietor knows more than she's sharing

### Session Prep Checklist
- [ ] Review NPC relationship status with party
- [ ] Check artifact locations and ownership
- [ ] Plan supernatural encounters based on investigation direction
- [ ] Prepare atmospheric descriptions for chosen locations

---

*Last Updated: 2025-08-10*  
*Campaign Status: Active - Session 2 completed*