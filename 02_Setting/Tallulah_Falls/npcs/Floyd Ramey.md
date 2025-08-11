---
type: npc
created: 2025-08-11
updated: 2025-08-11
tags:
  - npc
home_location: "[[Tallulah Falls]]"
current_location: "[[Train Car]]"
notable_locations:
  - "[[Train Car]]"
faction: Tallulah Falls Railway
trust_level: friendly
character_type: local
knowledge_level: aware
status: alive
relationships:
---

# Floyd Ramey

**First Appearance:**  
Floyd can be found in the train-car while the PCs make the journey into town. He can be found stationed at the Depot most times a train is in town. he lives in the worker part of town (to be described later)

## Description
- **Physical appearance:** He would be six foot exactly if age hadn't bent his back over the past decade. His face is rough with age, sporting a trimmed salt & peppered beard, his green eyes twinkle with knowledge and are crowned at their edges with crows feet.
- **Personality:** Affable when dealing with paying passengers, but is able to hold his own against drifters or an belligerent passengers. Though he comes off as very deferential and personable to his passengers, he doesn't tolerate prying unless its a good yarn.  
- **Quirks/Mannerisms:** He's hunched over, and can be quite a character; especially if someone slips him some of ole' Fate's moonshine. 
- **Mountain accent/dialect:** Still settling on specific mannerisms and speaking style

## Background
- **Born/raised:** Born and raised near Dillard, further "up the line." Life was mostly farming until the railroad came through and offered decent wages.
- **Family connections:** Has a couple of siblings, though a few are dead now. At least one brother is still around helping their aging mother. His father died last year. Chose to stay lonesome, as his love for the freedom that being connected to the rails provided kept him from settling down, though he never left these mountains - having seen some of the world, he couldn't find the bravery to fully leave these mountains he calls home.
- **Occupation:** Railroad conductor. Started by literally helping lay the tracks, then worked the mail train tendering the post before achieving his current position as conductor.
- **Local reputation:** Highly respected by those on the railroad since he not only did the cushy jobs - he started laying track and clearing land, bled and sweat for the road. Mostly overlooked by the rich patrons who only visit in the summer, but the long-timers and full-timers respect him and give him a nod and a wave on the street, or in an illegal saloon.

## Role in Campaign
- **Motivation:** Wants to keep the mountains open - he likes people coming to see the beauty and the green he grew up in. Functions as a helpful "bulletin board" for information in a natural, organic way.
- **Goals:** Protect the mountains and tourism, keep the trains running, help folks who seem genuinely lost or in trouble.
- **Secrets:** With all those years of listening to passengers and seeing people come and go, Floyd carries various secrets overheard during his work - information that might slip out when he's had some of Fate's moonshine.
- **What they know about the Old Gods:** He's got stories to tell, but he just sees them as stories. Like his father, he's practical and has no time for "granny magic" and "stories" as he'd call them. To him, they are nothing but tall tales, though damned if he doesn't know most of them. "Woods have been scaring people for eternity, and these woods ain't any scarier than any others I've heard of."

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

- **Allies:** Fellow railroad workers, long-time locals and full-timers who respect his service
- **Rivals/Enemies:** None specific
- **Family:** Aging mother and at least one brother still alive near Dillard; father died last year
- **Professional contacts:** Fate (the moonshiner, based on William Lafayette "Fate" Free)

## Old Gods Connection
- **Awareness level:** High knowledge of local folklore and "tall tales" but complete skepticism about their supernatural truth
- **Personal encounters:** Dismisses any strange experiences with practical explanations
- **Family history:** Father was similarly practical and dismissive of supernatural stories
- **Warnings they might give:** Practical warnings only - mountain lions, dangerous terrain, getting lost after dark, treacherous river conditions, avoiding certain people when they've been drinking

## Session Appearances
```dataview
TABLE without id file.link as "Session", date as "Date", role_played as "Role in Session"
FROM #session
WHERE contains(npcs_encountered, "[[" + this.file.name + "]]")
```

## Mechanics
- **Tier:** Capable
- **Key abilities:** Local knowledge, people skills, basic self-defense
- **Equipment:** Pocket watch, diary in his vest, passenger/luggage manifest, pocket knife
- **Combat notes:** Generally tries to use charisma to talk situations down, but knows how to use his pocket knife in emergencies. Physical presence from his track-laying days.

## Dialogue & Voice
- **Sample phrases:** Still developing specific mountain dialect and expressions
- **Speaking style:** More animated and theatrical when he's had some of Fate's moonshine, leaning into the storytelling aspect
- **Topics they avoid:** None specifically - will share information naturally, especially when loosened up by moonshine

## GM Notes
**Plot hooks:**
- Natural source for information about who's in town, best places to look for things/people
- Overhears conversations from passengers, notices strange cargo shipments, nervous travelers
- Can point PCs toward adventure through his extensive knowledge of local people and places
- When drinking, might slip out information like Hagrid in Harry Potter

**Future plans:**
- Open to developing relationship with PCs if they prove they genuinely care about the mountains and people
- Can become more personally invested in adventures that align with protecting the mountains and tourism

**If they turn hostile:**
- Would take significant provocation given his generally helpful nature
- Likely scenarios: threats to the railroad, the mountains, or people he cares about
