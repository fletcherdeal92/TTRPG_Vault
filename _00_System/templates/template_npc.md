---
type: npc
created: <% tp.file.creation_date("YYYY-MM-DD") %>
updated: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - npc
home_location: "[[]]"
current_location: "[[]]"
notable_locations: []
faction: 
trust_level: 
character_type: 
knowledge_level: 
status:
relationships: []
---

# <% tp.file.title %>

**First Appearance:**  
<% tp.file.cursor(1) %>

## Description
- **Physical appearance:** 
- **Personality:** 
- **Quirks/Mannerisms:** 
- **Mountain accent/dialect:** 

## Background
- **Born/raised:** 
- **Family connections:** 
- **Occupation:** 
- **Local reputation:** 

## Role in Campaign
- **Motivation:** 
- **Goals:** 
- **Secrets:** 
- **What they know about the Old Gods:** 

## Location Information
**Home:** `=this.home_location`  
**Currently at:** `=this.current_location`  
**Notable places:** `=this.notable_locations`

```dataview
TABLE without id file.link as "Location", location_type as "Type", danger_level as "Safety"
FROM #location
WHERE "[[" + this.file.name + "]]" = current_location OR contains(notable_locations, "[[" + this.file.name + "]]") OR "[[" + this.file.name + "]]" = home_location
```

## Relationships
```dataview
TABLE without id file.link as "Connected NPC", faction as "Faction", trust_level as "Trust"
FROM #npc
WHERE contains(relationships, "[[" + this.file.name + "]]")
```

- **Allies:** 
- **Rivals/Enemies:** 
- **Family:** 
- **Professional contacts:** 

## Old Gods Connection
- **Awareness level:** 
- **Personal encounters:** 
- **Family history:** 
- **Warnings they might give:** 

## Session Appearances
```dataview
TABLE without id file.link as "Session", date as "Date", role_played as "Role in Session"
FROM #session
WHERE contains(npcs_encountered, "[[" + this.file.name + "]]")
```

## Mechanics
- **Tier:** 
- **Key abilities:** 
- **Equipment:** 
- **Combat notes:** 

## Dialogue & Voice
- **Sample phrases:** 
- **Speaking style:** 
- **Topics they avoid:** 

## GM Notes
**Plot hooks:**
- 

**Future plans:**
- 

**If they turn hostile:**
- 
