---
type: npc
created: <% tp.file.creation_date("YYYY-MM-DD") %>
updated: <% tp.date.now("YYYY-MM-DD") %>
tags: [npc]
location: 
faction: 
trust_level: # hostile/wary/neutral/friendly/allied
character_type: # local/outsider/supernatural/cultist/authority
knowledge_level: # ignorant/suspicious/aware/involved/corrupted
status: # alive/missing/dead/transformed
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

## Relationships
```dataview
TABLE without id file.link as "Connected NPC", relationship as "Relationship"
FROM #npc
WHERE contains(relationships, this.file.name)
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
WHERE contains(npcs_encountered, this.file.name)
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
