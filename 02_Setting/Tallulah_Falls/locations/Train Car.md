---
type: location
created: 2025-08-11
updated: 2025-08-11
tags:
  - location
location_type: transportation
parent_location: "[[Depot]]"
region: Tallulah Falls
settlement_type: none
danger_level: safe
population: 0
primary_industry: none
old_gods_influence: 
artifacts_found: 
special_rules:
---

# Train Car
  Make every PCs introduction connect them to the scene and character. 
  
 >[!gm] Introduction Example
 >*i.e.* Mr. James Ellis, sits on a wooden bench, the sweltering summer sun hits his arm through the window he leans against as the steady rocking of the old TF nearly put him to sleep. It's been a while since he's been home.
  
  This is our introduction to the world. Westworld got it right when it starts you off on a train journey. There's something about being part of that. even in your head imagining taking that train can bridge the gap in our head and hearts. 

## Description
- **Physical layout:** The Train car is your standard for the time, if a little dated. The consist of this tourist run consists of a baggage car followed by four passenger cars, each filled with travelers from all parts. Our PCs find themselves in the 3rd passenger car. Standing in the back of the car facing forward in the direction of travel ones eye would follow the well worn aisle to the far end of the car where a pot bellied stove sits unused in the sweltering summer heat to the left of the aisle, opposite of it is a communal water stand, focusing wider you'd start to notice the deep oak paneled car surrounding you in almost a warm hug from the light coming through the 20 windows on each side of the car, each window consisting of a row of "walkover" bench seats that could switch directions with the train. these seats were plain, in the same lacquered oak as the rest of the panelling. Looking up into the clerestory of the train you notice the curved ceiling is painted white, causing the light from the windows in the raised section of the roof to glow. To your right is the privy, at this time practically a hole in the floor with a seat. At least its separated from the rest of the car. To your left is a moderately sized man in his seat, hunched over and looking at what appears to be a passenger manifest.
- **Atmosphere:** The atmosphere on the train changes. When the characters "start" their journey at cornelia (only connection to any other line) its sweltering, as the train travels further into the green and the mountains, a chill rises. Once they reach the gorge, those who are first timers discover why this area used to be noted as the place "Where spring spends the summer." There's is joy and excitement for most of the journey. We jump int right before panther creek trestle which casuses some unease in passengers, some remembering the accident from 10 years ago and praying it doesn't happen again. Other's from what they fear is outside the windows, in the woods.
- **Notable features:** N/A
- **Local folklore:** There is nothing associated with this specific train

## History & Background
- **Founded/discovered:** Has been a consist of the TFRR for 20 years, it was not involved in the accident. It has had a relatively trouble free existence.

## Supernatural Elements
- **Strange occurrences:** possible in the future
- **Local legends:** possible in the future
- **Warning signs:** n/a

## NPCs Present Here
```dataview
TABLE without id file.link as "Name", faction as "Faction", trust_level as "Trust"
FROM #npc
WHERE current_location = link(this.file.name)
```

## NPCs From Here
```dataview
TABLE without id file.link as "Name", faction as "Faction", current_location as "Currently At"
FROM #npc
WHERE home_location = link(this.file.name)
```

## NPCs Who Visit Here
```dataview
TABLE without id file.link as "Name", faction as "Faction", trust_level as "Trust"
FROM #npc
WHERE contains(notable_locations, link(this.file.name))
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
WHERE contains(locations_visited, "[[" + this.file.name + "]]")
```


## GM Notes
**Secrets:**
- 

**Foreshadowing:**
- 

**Environmental Hazards:**
- 
