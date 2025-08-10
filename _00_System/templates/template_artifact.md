---
type: artifact
created: <% tp.file.creation_date("YYYY-MM-DD") %>
updated: <% tp.date.now("YYYY-MM-DD") %>
tags: [artifact]
category: # mundane/occult/cursed/blessed/technological
danger_level: # safe/caution/dangerous/lethal/reality_warping
current_location: 
original_location: 
discovery_session: 
discovered_by: []
current_owner: 
value: # monetary value in 1920s dollars
rarity: # common/uncommon/rare/unique/legendary
old_gods_connection: # none/minor/moderate/strong/direct
---

# <% tp.file.title %>

<% tp.file.cursor(1) %>

## Description
- **Physical appearance:** 
- **Size/weight:** 
- **Materials:** 
- **Condition:** 
- **Age:** 

## History & Origin
- **Created when:** 
- **Created by:** 
- **Original purpose:** 
- **How it came to this location:** 
- **Previous owners:** 

## Discovery
- **Found where:** 
- **Found when:** 
- **Found by:** 
- **Circumstances:** 
- **Initial reaction:** 

## Properties & Effects

### Mundane Properties
- **Practical use:** 
- **Monetary value:** 
- **Historical significance:** 

### Supernatural Properties
- **Mystical effects:** 
- **Activation requirements:** 
- **Duration of effects:** 
- **Side effects:** 
- **Corruption risk:** 

## Old Gods Connection
- **Which entity:** 
- **Type of connection:** 
- **Influence level:** 
- **Warning signs:** 
- **Protective measures needed:** 

## Game Mechanics

### Cypher System Stats
- **Level:** 
- **Form:** 
- **Effect:** 
- **Depletion:** 

### Special Rules
- **Usage limitations:** 
- **Skill requirements:** 
- **Environmental effects:** 
- **Interaction with other items:** 

## Associated NPCs
```dataview
TABLE without id file.link as "NPC", relationship as "Connection", knowledge_level as "What They Know"
FROM #npc
WHERE contains(connected_artifacts, this.file.name)
```

## Associated Locations
```dataview
TABLE without id file.link as "Location", connection_type as "Connection"
FROM #location
WHERE contains(artifacts_found, this.file.name)
```

## Session History
```dataview
TABLE without id file.link as "Session", date as "Date", event as "What Happened"
FROM #session
WHERE contains(artifacts_involved, this.file.name)
```

## Research & Investigation
### What Can Be Learned
- **Easy to discover (Difficulty 2):** 
- **Moderate research (Difficulty 4):** 
- **Deep investigation (Difficulty 6):** 
- **Forbidden knowledge (Difficulty 8):** 

### Research Sources
- **Local folklore:** 
- **Historical records:** 
- **Academic sources:** 
- **Occult texts:** 
- **Witnesses:** 

## Warnings & Precautions
### Handling Safely
- **Physical precautions:** 
- **Spiritual protections:** 
- **Time limitations:** 
- **Environmental needs:** 

### Signs of Corruption
- **User effects:** 
- **Environmental effects:** 
- **Social effects:** 
- **Reality distortions:** 

## Plot Hooks
### Current Storylines
- 
- 
- 

### Future Possibilities
- 
- 
- 

## GM Notes
### Campaign Integration
- **Role in main plot:** 
- **Connection to other artifacts:** 
- **Long-term consequences:** 

### If Players Abuse It
- **Safeguards:** 
- **Escalating consequences:** 
- **Removal methods:** 

### Secrets
- **Hidden properties:** 
- **True origin:** 
- **Connections unknown to players:** 

---

## Quick Reference
**Danger:** 
**Use:** 
**Warning:** 
**Value:** $