---
type: session
created: <% tp.file.creation_date("YYYY-MM-DD") %>
updated: <% tp.date.now("YYYY-MM-DD") %>
tags: [session]
session_number: 
date: <% tp.date.now("YYYY-MM-DD") %>
duration: # hours
campaign: Written_in_Water
adventure_arc: 
players_present: []
locations_visited: []
npcs_encountered: []
artifacts_discovered: []
---

# Session <% tp.file.title %> - <Adventure Title>

**Date:** <% tp.date.now("YYYY-MM-DD") %>  
**Duration:** X hours  
**Players Present:** 

<% tp.file.cursor(1) %>

## Pre-Session Setup
### GM Preparation
- [ ] Review previous session notes
- [ ] Prepare NPC voices and personalities
- [ ] Set up battle maps/handouts
- [ ] Review rules questions from last time

### Player Recap
**What happened last session:**
- 
- 
- 

## Session Goals
- **Primary objective:** 
- **Secondary objectives:** 
- **Character development focus:** 

## Locations Visited
```dataview
TABLE without id file.link as "Location", location_type as "Type", danger_level as "Danger"
FROM #location
WHERE contains(this.locations_visited, "[[" + file.name + "]]")
```

## NPCs Encountered
```dataview
TABLE without id file.link as "NPC", faction as "Faction", trust_level as "Trust"
FROM #npc
WHERE contains(this.npcs_encountered, "[[" + file.name + "]]")
```

## Artifacts & Items
### Discovered This Session
- artifacts_discovered: []

### Used/Given to Players
- items_given: []

```dataview
TABLE without id file.link as "Item", type as "Type", current_location as "Now Located"
FROM #artifact
WHERE contains(this.artifacts_discovered, "[[" + file.name + "]]")
```

## Key Events & Scenes

### Opening Scene
**Location:** 
**Setup:** 
**Player actions:** 

### Major Encounters
#### Encounter 1: [Name]
**Type:** Social/Combat/Investigation/Supernatural
**Location:** 
**NPCs involved:** 
**Outcome:** 
**Clues revealed:** 

#### Encounter 2: [Name]
**Type:** 
**Location:** 
**NPCs involved:** 
**Outcome:** 
**Clues revealed:** 

### Closing Scene
**Location:** 
**Cliffhanger/Setup:** 

## Old Gods Elements
### Supernatural Encounters
- **Strange occurrences:** 
- **Folklore revealed:** 
- **Warnings given:** 
- **Corruption witnessed:** 

### Mounting Tension
- **Unease level:** 1-10
- **Player paranoia:** 
- **Environmental horror:** 

## Character Development
### Individual Character Moments
- **[Character Name]:** 
- **[Character Name]:** 
- **[Character Name]:** 

### Party Dynamics
- **Trust building:** 
- **Conflicts:** 
- **Shared experiences:** 

## Rules & Mechanics
### New Rules Introduced
- 
- 

### Rules Questions
- **Question:** 
  **Ruling:** 

### Experience & Advancement
- **XP awarded:** 
- **Milestones reached:** 
- **Character advancements:** 

## Player Feedback
### What Worked Well
- 
- 

### What to Improve
- 
- 

### Player Questions
- 
- 

## GM Notes & Reflections
### Pacing
- **Too fast/slow moments:** 
- **Best paced scenes:** 

### NPC Performance
- **Well-received NPCs:** 
- **NPCs to develop more:** 

### Plot Threads
- **Advanced this session:** 
- **Need attention next time:** 

## Foreshadowing & Setup
### Seeds Planted
- 
- 

### Mysteries Deepened
- 
- 

## Next Session Preparation
### Immediate Followup
- [ ] Resolve cliffhanger
- [ ] Address player questions
- [ ] Follow up on character moments

### NPCs to Prepare
- 
- 

### Locations to Detail
- 
- 

### Props/Handouts Needed
- 
- 

## Session Summary
**One sentence summary:** 

**Key developments:**
- 
- 
- 

**Cliffhanger:** 

---

## Quick Reference
**Session Number:** 
**Campaign Day:** 
**In-game Date:** 
**Weather:** 
**Season:** Fall 1923