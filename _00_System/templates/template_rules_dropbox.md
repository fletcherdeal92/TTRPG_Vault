---
type: rule
created: <% tp.file.creation_date("YYYY-MM-DD") %>
updated: <% tp.date.now("YYYY-MM-DD") %>
tags: [rule]
category: # core/house/clarification/optional/supernatural
complexity: # simple/moderate/complex
frequency: # constant/common/situational/rare
system: # cypher/ogoa/universal
applies_to: # combat/social/investigation/supernatural/general
---

# <% tp.file.title %>

<% tp.file.cursor(1) %>

## Rule Summary
**Quick reference:** 

## Detailed Explanation
### When This Rule Applies
- 
- 
- 

### How It Works
1. 
2. 
3. 

### Examples
**Example 1:**
- **Situation:** 
- **Application:** 
- **Outcome:** 

**Example 2:**
- **Situation:** 
- **Application:** 
- **Outcome:** 

## Old Gods of Appalachia Integration
### Setting-Specific Applications
- **Mountain folklore:** 
- **Supernatural encounters:** 
- **1920s technology limitations:** 
- **Community dynamics:** 

### Atmospheric Considerations
- **Building tension:** 
- **Maintaining mystery:** 
- **Cultural authenticity:** 

## Mechanical Details

### Cypher System Integration
- **Difficulty modifications:** 
- **Asset/hindrance rules:** 
- **GM intrusion opportunities:** 
- **Edge cases:** 

### Related Rules
```dataview
TABLE without id file.link as "Related Rule", category as "Category", relationship as "How They Connect"
FROM #rule
WHERE contains(related_rules, this.file.name)
```

### Conflicts & Clarifications
- **Overrides:** 
- **Exceptions:** 
- **Edge cases:** 
- **GM discretion points:** 

## Session Applications
### Quick Reference Table
| Situation | Difficulty | Modifier | Notes |
|-----------|------------|----------|-------|
|           |            |          |       |
|           |            |          |       |
|           |            |          |       |

### GM Tools
- **When to apply:** 
- **When to ignore:** 
- **Scaling for drama:** 
- **Player agency considerations:** 

## Common Mistakes
### Player Misunderstandings
- **Common error:** 
  **Correction:** 

- **Common error:** 
  **Correction:** 

### GM Pitfalls
- **Avoid:** 
  **Instead:** 

- **Avoid:** 
  **Instead:** 

## Playtesting Notes
### What Works Well
- 
- 

### What Needs Adjustment
- 
- 

### Player Feedback
- 
- 

## Related Content
### NPCs That Use This Rule
```dataview
TABLE without id file.link as "NPC", location as "Location", notes as "How They Use It"
FROM #npc
WHERE contains(special_rules, this.file.name)
```

### Locations Where It Applies
```dataview
TABLE without id file.link as "Location", region as "Region", application as "How Rule Applies"
FROM #location
WHERE contains(special_rules, this.file.name)
```

### Sessions That Featured This Rule
```dataview
TABLE without id file.link as "Session", date as "Date", usage as "How It Was Used"
FROM #session
WHERE contains(rules_used, this.file.name)
```

## Designer Notes
### Intent
**Purpose:** 
**Design goals:** 
**Inspiration:** 

### Balance Considerations
- **Power level:** 
- **Complexity cost:** 
- **Fun factor:** 
- **Narrative support:** 

## Variants & Options
### Simplified Version
- **When to use:** 
- **How it works:** 

### Advanced Version
- **When to use:** 
- **Additional complexity:** 

### Optional Additions
- 
- 

---

## Quick Reference Card
**Rule:** 
**When:** 
**How:** 
**Difficulty:** 
**Special:** 