# Security+ (SY0-701) Obsidian Study Vault

A complete Obsidian vault for studying CompTIA Security+ (SY0-701), built around Professor Messer's free video course. Meant to be cloned/copied as a starting template for other certs and courses too.

## What's in it

- **[[00 - CompTIA Objectives Summary]]** — the official exam scope, weighted by domain
- **[[01 - Contents]]** — full clickable table of contents, one checkbox per Messer video, in his exact course order, with a live per-domain and overall progress bar
- **5 domain overview pages** (1.0–5.0), each linking to every topic underneath it
- **120 individual topic notes**, one per video/section, each with a `confidence` field (blank / solid / shaky / missed) plus a Practice gaps section for tracking what you got wrong and why
- **`Daily Notes/`** — a day-by-day schedule (Aug 4–28) with each day's study blocks written as checkbox tasks with due dates, built for the Calendar and Tasks plugins
- **`Weekly Board.md`** — a Kanban board (one card per study day) for a coarser week-level view, for the Kanban plugin
- **Home.md** — the front page tying all of the above together

## Setup

Install these from Settings → Community plugins → Browse (search each by name, Install, then Enable):

1. **Dataview** — powers the progress bars in Contents and Home. After installing, go to Settings → Dataview and turn on **"Enable JavaScript Queries."** Without this plugin the checkboxes still work fine, you just won't get the auto-counted bars.
2. **Daily notes** — this is a *core* plugin (Settings → Core plugins, not Community), just toggle it on. Set its **New file location** to `Daily Notes` and its **date format** to `YYYY-MM-DD` — this vault's daily notes already match that naming.
3. **Calendar** — no config needed. Open its pane from the calendar-grid icon in the left ribbon, or Ctrl/Cmd+P → "Open calendar." Every study day (Aug 4–28) shows a dot; click a date to open that day's plan.
4. **Tasks** — no config needed. It reads the 📅 due-date tags already sitting on every block checkbox in `Daily Notes/`.
5. **Kanban** — no config needed. Open `Weekly Board.md` and it should render as a drag-and-drop board, not plain text.

## How to use this as a template for a different cert

1. Copy the vault folder, rename it.
2. Replace the objectives list in `00 -` and the section list in `01 - Contents` with the new exam's structure.
3. Regenerate `Notes/`, `Daily Notes/`, and `Weekly Board.md` to match — or just hand-edit if the new cert is smaller.

## License

Personal study notes — copy, fork, and adapt freely.
