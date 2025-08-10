# Faction Relationships - Old Gods of Appalachia

*Tracking the complex web of relationships between different groups in and around Tallulah Falls*

## Faction Overview

### Local Townspeople
**Description:** Established mountain community families who've lived in the area for generations  
**Goals:** Preserve community safety and traditional way of life  
**Secrets:** Maintain protective folklore and know which areas to avoid  
**Relationship to Supernatural:** Aware but prefer to ignore/avoid rather than confront  

### Outsiders
**Description:** Visitors, researchers, government agents, and other non-locals  
**Goals:** Various - research, business, tourism, investigation  
**Secrets:** Often unaware of supernatural dangers they're walking into  
**Relationship to Supernatural:** Range from complete ignorance to dangerous obsession  

### Old Families
**Description:** Cherokee descendants and families with multi-generational supernatural knowledge  
**Goals:** Protect the balance between worlds, maintain protective traditions  
**Secrets:** Hold the deepest knowledge of Old Gods activity and protection methods  
**Relationship to Supernatural:** Respectful awareness and active protection practices  

### Economic Interests
**Description:** Railroad companies, dam construction, tourism developers  
**Goals:** Profit from natural resources and geographic features  
**Secrets:** Will suppress supernatural incidents that threaten business interests  
**Relationship to Supernatural:** Dismissive, actively cover up incidents  

---

## Faction Relationships Matrix

| Faction | Local Townspeople | Outsiders | Old Families | Economic Interests |
|---------|-------------------|-----------|-------------|-------------------|
| **Local Townspeople** | Cooperative | Wary | Respectful | Cautious |
| **Outsiders** | Dismissive | Competitive | Ignorant | Aligned |
| **Old Families** | Protective | Warning | Traditional | Opposed |
| **Economic Interests** | Exploitative | Opportunistic | Hostile | Competitive |

---

## Faction Members

### Local Townspeople
```dataview
TABLE WITHOUT ID
  file.link as "NPC",
  location as "Location",
  trust_level as "Attitude to PCs",
  knowledge_level as "Supernatural Awareness"
FROM #npc
WHERE faction = "Local Townspeople"
SORT location ASC, trust_level DESC
```

### Outsiders
```dataview
TABLE WITHOUT ID
  file.link as "NPC",
  location as "Current Location",
  character_type as "Type",
  status as "Current Status"
FROM #npc
WHERE faction = "Outsiders"
SORT status ASC, character_type ASC
```

### Old Families
```dataview
TABLE WITHOUT ID
  file.link as "NPC",
  location as "Territory",
  knowledge_level as "Supernatural Knowledge",
  trust_level as "Willingness to Help"
FROM #npc
WHERE faction = "Old Families" OR faction = "Cherokee Descendants"
SORT knowledge_level DESC
```

### Economic Interests
```dataview
TABLE WITHOUT ID
  file.link as "NPC",
  location as "Base of Operations",
  character_type as "Role",
  trust_level as "Attitude"
FROM #npc
WHERE faction = "Railroad Company" OR faction = "Dam Construction" OR faction = "Tourism"
SORT character_type ASC
```

---

## Relationship Dynamics

### Cooperation Patterns
- **Local Townspeople + Old Families**: Share protective knowledge, respect boundaries
- **Outsiders + Economic Interests**: Often work together for development projects
- **Old Families + Local Townspeople**: Multi-generational alliances and intermarriage

### Conflict Patterns
- **Economic Interests vs. Old Families**: Development threatens sacred/protected sites
- **Outsiders vs. Local Townspeople**: Cultural misunderstanding and suspicion
- **Economic Interests vs. Local Townspeople**: Exploitation of local resources and labor

### Protection Networks
- **Local Warning Systems**: Informal networks share information about supernatural dangers
- **Economic Suppression**: Business interests actively cover up supernatural incidents
- **Traditional Protections**: Old Families maintain rituals and boundary markings

---

## Supernatural Awareness Levels

### Highly Aware (Active Knowledge)
```dataview
TABLE WITHOUT ID
  file.link as "NPC",
  faction as "Faction",
  knowledge_level as "Awareness Type"
FROM #npc
WHERE knowledge_level = "involved" OR knowledge_level = "corrupted"
SORT faction ASC
```

### Moderately Aware (Suspicious/Cautious)
```dataview
TABLE WITHOUT ID
  file.link as "NPC",
  faction as "Faction",
  knowledge_level as "Awareness Type"
FROM #npc
WHERE knowledge_level = "aware" OR knowledge_level = "suspicious"
SORT faction ASC
```

### Unaware/Ignorant
```dataview
TABLE WITHOUT ID
  file.link as "NPC",
  faction as "Faction",
  knowledge_level as "Awareness Type"
FROM #npc
WHERE knowledge_level = "ignorant"
SORT faction ASC
```

---

## Trust Relationship Tracking

### Allied to Party
```dataview
TABLE WITHOUT ID
  file.link as "NPC",
  faction as "Faction",
  location as "Where to Find"
FROM #npc
WHERE trust_level = "allied"
SORT faction ASC
```

### Friendly to Party
```dataview
TABLE WITHOUT ID
  file.link as "NPC",
  faction as "Faction",
  location as "Where to Find"
FROM #npc
WHERE trust_level = "friendly"
SORT faction ASC
```

### Neutral to Party
```dataview
TABLE WITHOUT ID
  file.link as "NPC",
  faction as "Faction",
  location as "Where to Find"
FROM #npc
WHERE trust_level = "neutral"
SORT faction ASC
```

### Wary/Hostile to Party
```dataview
TABLE WITHOUT ID
  file.link as "NPC",
  faction as "Faction",
  trust_level as "Specific Attitude"
FROM #npc
WHERE trust_level = "wary" OR trust_level = "hostile"
SORT trust_level ASC, faction ASC
```

---

## Faction Goals & Motivations

### Local Townspeople
- **Primary Goal:** Maintain community safety and prosperity
- **Secondary Goals:** Preserve traditional ways, protect family secrets
- **Fears:** Economic exploitation, supernatural exposure, loss of community
- **Resources:** Local knowledge, established networks, practical skills

### Outsiders
- **Primary Goal:** Achieve individual objectives (research, profit, tourism)
- **Secondary Goals:** Understand local culture, gain acceptance
- **Fears:** Local hostility, supernatural dangers, failure of mission
- **Resources:** Education, technology, outside connections, money

### Old Families
- **Primary Goal:** Maintain balance between supernatural and mundane worlds
- **Secondary Goals:** Protect sacred sites, preserve traditional knowledge
- **Fears:** Supernatural corruption, loss of protective traditions, exploitation of sacred knowledge
- **Resources:** Ancient knowledge, spiritual protection, connection to land

### Economic Interests
- **Primary Goal:** Maximize profit from natural resources and geography
- **Secondary Goals:** Minimize obstacles to development, maintain public image
- **Fears:** Bad publicity, government intervention, supernatural interference with operations
- **Resources:** Money, political connections, technology, legal power

---

## Faction Interaction Guidelines

### Gaining Local Townspeople Trust
- Show respect for local customs and knowledge
- Demonstrate genuine concern for community welfare
- Avoid appearing to exploit or judge local ways
- Offer practical help with community problems

### Working with Old Families
- Approach with proper respect and humility
- Demonstrate understanding of supernatural dangers
- Show willingness to learn and follow protective traditions
- Never demand or try to steal sacred knowledge

### Managing Economic Interests
- Understand they prioritize profit over everything else
- Be prepared for attempts at bribery or coercion
- Recognize they will suppress supernatural evidence
- May be valuable allies if interests align

### Dealing with Other Outsiders
- Fellow researchers may share information freely
- Government agents may have competing agendas
- Tourists are generally oblivious but may witness events
- Some outsiders may be supernatural entities in disguise

---

## Current Faction Status

### Local Townspeople
**Current Mood:** Cautiously welcoming to Player Characters due to Professor Whitaker connection  
**Recent Events:** Increased supernatural activity has everyone on edge  
**Key Issues:** Worried about missing Professor, concerned about increased outsider attention  

### Old Families
**Current Mood:** Watchful and evaluating - haven't yet determined if PCs can be trusted with deeper knowledge  
**Recent Events:** Supernatural activity suggests something major approaching  
**Key Issues:** Debating whether to share protective knowledge with newcomers  

### Economic Interests
**Current Mood:** Business as usual, suppressing any supernatural reports  
**Recent Events:** Railroad schedules maintained despite worker unease  
**Key Issues:** Need to keep supernatural incidents from affecting business operations  

---

*Last Updated: 2025-08-10*  
*Note: Faction relationships may evolve based on PC actions and campaign developments*