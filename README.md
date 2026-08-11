# Security+ (SY0-701) Obsidian Study Vault

A custom Obsidian study vault for CompTIA Security+ (SY0-701), organized around the official CompTIA exam objectives and Professor Messer's course order. Needed something to organize my approach to studying, as well as create a visual progress meter as I made my way through course material.

## What's included

- `00 - CompTIA Objectives Summary.md` — official domain weighting and scope
- `01 - Contents.md` — clickable topic list in Professor Messer's course order with progress tracking
- Domain overview pages for Domains 1–5
- Individual topic notes with confidence tracking and practice-gap sections
- `Daily Notes/` — the day-by-day study schedule and task driver
- `Weekly Board.md` — week-level Kanban view
- `Study Method.md` — how to work through each study day
- `Home.md` — vault landing page
- `References.md` — source and study-resource references

## Installation

1. Download or clone the repository.
2. Open Obsidian.
3. Choose **Open folder as vault**.
4. Select the downloaded vault folder.

## Required Obsidian plugins

Install and enable:

- **Dataview**
- **Tasks**
- **Calendar**
- **Kanban**

Recommended if you want the vault to match the original setup:

- Advanced Tables
- Git
- Style Settings
- Day Planner

### Dataview setup

After installing Dataview:

1. Open **Settings → Dataview**.
2. Enable **JavaScript Queries**.

The progress bars in `Home.md` and `01 - Contents.md` depend on this setting.

### Daily Notes setup

Obsidian's built-in **Daily Notes** core plugin should be enabled.

Set:

- **New file location:** `Daily Notes`
- **Date format:** `YYYY-MM-DD`

The prebuilt daily files already use that naming convention.

## How to use the vault

Start from `Home.md`.

Use `01 - Contents.md` as the master topic tracker. The topic order follows Professor Messer's SY0-701 course sequence.

The daily study plan lives in `Daily Notes/`. Open the note for the current date through the Calendar plugin or directly from the folder. Each daily note contains that day's study tasks and due dates.

After completing the study workflow for a topic, check it off in `01 - Contents.md`. The Dataview progress bars update automatically.

## Confidence tracking

Each individual topic note includes a `confidence` field.

Use:

- `solid` — you can answer correctly without hesitation
- `shaky` — partly correct, slow, or uncertain
- `missed` — incorrect

Leave it blank until you've actually tested yourself on the topic.

For anything marked `shaky` or `missed`, add a short note under **Practice gaps** describing the specific concept you confused or forgot.

You can search Obsidian for:

- `confidence: shaky`
- `confidence: missed`

That gives you a ready-made review queue.

## Study structure

The vault is designed around two things:

1. **CompTIA's SY0-701 exam objectives** define what is in scope and how heavily each domain is weighted.
2. **Professor Messer's course order** determines the sequence used for learning topics.

The daily schedule spreads that material across smaller learning blocks and includes recall before moving on. Practice and gap repair become heavier after the first pass through the content.

The schedule itself is contained in the files under `Daily Notes/`; there is no separate master schedule file to maintain.

## Using this vault for another certification

You can reuse the structure for another certification:

1. Copy the vault.
2. Replace the objective summary.
3. Replace the topic list in `01 - Contents.md`.
4. Update the domain overview pages.
5. Replace the topic notes.
6. Rebuild the files under `Daily Notes/` and update `Weekly Board.md`.

## Sources and attribution

CompTIA Security+ and SY0-701 are trademarks of CompTIA, Inc.

Professor Messer course structure, video titles, and course-note references belong to Messer Studios, LLC.

This vault is an independent personal study framework and does not reproduce the full contents of CompTIA exam materials or Professor Messer's paid course notes.
