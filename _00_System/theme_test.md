---
type: test
created: 2025-08-12
updated: 2025-08-12
tags: 
  - cosmic-horror
  - ancient
  - whisper
  - eldritch
  - trusted
  - suspicious
  - neutral
trust_level: trusted
faction: Old Gods
---

# Session 01: The Gorge Overlook Theme Test

Welcome to the **Old Gods of Appalachia** theme showcase! This file demonstrates all the custom styling features added to the *Gorge Overlook* theme.

## Headers and Typography

# H1 Header (Session Style)
## H2 Header - Sage Green
### H3 Header - Also Sage Green  
#### H4 Header - Bright Neutral
##### H5 Header - Muted Text
###### H6 Header - Also Muted

**Bold text** should use the sandy beige color, while *italic text* uses muted tones.

## Dice Notation Highlighting

Roll for investigation: `1d20+3`
Damage from the ancient force: `2d6+1` 
Sanity check: `1d100`
Multiple dice: `4d6`, `1d8`, `2d10+5`

## Stat Block Example (Blockquote)

> **Elder Thing of the Gorge**
> 
> **Health:** 15
> **Armor:** 2 
> **Damage:** `1d8+2` (claws)
> **Special:** Whispers of madness - forces Sanity check `1d20` vs DC 15
> 
> *An ancient being that dwells in the deepest parts of Tallulah Gorge, its form shifts between shadow and substance.*

## Horror Atmosphere Tags

These tags should have a subtle glow effect:
#npc 
- #cosmic-horror 
- #ancient
- #whisper  
- #eldritch

## NPC Trust Level Examples

The frontmatter shows trust level indicators. Here are examples of how different trust levels should appear in tags:

**Floyd Ramey:** #trusted - Should appear in sage green
**Strange Stranger:** #suspicious - Should appear in reddish brown  
**Town Mayor:** #neutral - Should appear in sandy beige
**The Watchers:** #untrusted - Should appear in reddish brown

## Callout Examples

> [!handout] Player Handout
> This is what the players receive - a weathered letter found in Whitaker's belongings. The paper feels old and brittle, with faded ink that seems to shift in certain light.

> [!gm] GM Notes  
> The letter is actually written in a cipher that reveals the location of the underground complex. The players won't discover this unless they make a successful Intelligence check (DC 18) or consult historical records.

## Code and Technical Elements

Inline code like `whisper_check()` and `ancient_power.activate()` should stand out with the theme colors.

```markdown
# Example code block
function rollSanity() {
  return Math.floor(Math.random() * 20) + 1;
}
```

## Lists and Nested Content

- Primary list item
  - Nested item (should be muted)
    - Double nested (also muted)
      - Triple nested (sage green bullets)
- Another primary item
  - With nested content

1. Numbered list
   1. Nested numbered
      1. Double nested numbered

## Comments and Hidden Text

%%This is a GM comment that should appear muted and italic%%

Regular text continues here.

---

*This test file showcases all the TTRPG enhancements added to the Gorge Overlook theme for Old Gods of Appalachia campaigns.*