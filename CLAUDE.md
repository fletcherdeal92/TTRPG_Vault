# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a TTRPG (Tabletop Role-Playing Game) vault for running campaigns in the Old Gods of Appalachia setting. It's organized as a digital campaign notebook using markdown files with templating system.

## Repository Structure

The vault follows a numbered organizational system:

- `01_Rules_OGoA/` - Game rules, house rules, and reference materials
- `02_Setting/` - World setting information, locations, and lore
- `03_Adventures/` - Campaign adventures with sessions, props, and timelines  
- `04_Reference/` - Historical context, environmental notes, and period details
- `_00_System/` - Templates and system files for content creation

## Template System

The `_00_System/templates/` directory contains structured templates for consistent content creation:

- `template_npc.md` - Character creation with frontmatter for type, location, faction, trust_level
- `template_location.md` - Location entries with dataview queries for linked NPCs
- `template_session.md` - Session planning and notes
- `template_artifact.md` - Game items and artifacts
- `template_rules_dropbox.md` - Rules and mechanics

Templates use Templater plugin syntax (`<% tp.file.title %>`, `<% tp.file.cursor() %>`) and expect frontmatter with YAML metadata.

## Content Organization Patterns

- Files use descriptive names with spaces (e.g., "Town of Tallulah Falls.md")
- Frontmatter includes `type`, `created`, `updated`, `tags`, and content-specific fields
- Location files use dataview queries to dynamically link related NPCs
- Session files are numbered sequentially (session_00.md, session_01.md)
- Campaign materials are grouped by adventure arc

## Campaign Structure

The current campaign "Written in Water" is structured with:
- Campaign overview and timeline at adventure root
- Sessions organized in dedicated folder
- Props and handouts for players
- Setting details focused on 1920s Appalachian Georgia

This is a content-focused repository without build processes - all work involves editing markdown files and maintaining the organizational structure.