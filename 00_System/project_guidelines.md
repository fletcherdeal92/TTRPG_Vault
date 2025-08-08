# Project Guidelines (Agent Guardrails)

**Scope:**  
This repo is an Obsidian vault for an **Old Gods of Appalachia x Tallulah Falls** campaign. Only create/modify Markdown files inside the existing folders. Ask before deleting or moving files.

**Style:**  
- Every note has YAML frontmatter with at least: `title`, `type`, `tags`, `created`, `updated`.
- Use the templates in `00_System/templates/` for new notes.
- Keep sections short; use headings, bullets, and callouts.

**No-nos:**  
- Do not overwrite player handouts; if revising, create a new file with a `-v2` suffix.
- Do not change file names without updating links.

**Workflow:**  
1) Before large edits, present a short plan.  
2) After changes, show a git diff summary.  
3) Respect Templater variables if present (e.g., `<% tp.file.creation_date() %>`).

**DM Notes vs Player-Facing:**  
- Use `player_handout: true|false` in frontmatter.  
- GM-only notes go in `gm_notes` sections or `> [!gm]` callouts.

**Session Flow (text GMing):**  
I will frame scenes, ask for actions/rolls, and narrate outcomes. You (Elias) reply with intent + approach. We track clocks, harm, and intrusions inline.