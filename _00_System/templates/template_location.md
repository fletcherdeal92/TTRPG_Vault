---
type: location
created: <% tp.file.creation_date("YYYY-MM-DD") %>
updated: <% tp.date.now("YYYY-MM-DD") %>
tags: [location]
region: 
---

# <% tp.file.title %>

<% tp.file.cursor(1) %>

## Description
- Physical layout:  
- Atmosphere:  

## Notable NPCs
```dataview
TABLE description
FROM #npc
WHERE location = this.file.name
