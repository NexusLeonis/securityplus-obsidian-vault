# Security+ (SY0-701) — Home

Study vault for the CompTIA Security+ SY0-701 certification, built around Professor Messer's course order.

## Start here
- [[00 - CompTIA Objectives Summary]] — official exam weighting and scope, straight from CompTIA
- [[01 - Contents]] — full clickable table of contents, one link per topic, in Messer's video order

## Overall progress
```dataviewjs
const contents = dv.page("01 - Contents.md");
const tasks = contents.file.tasks;
const done = tasks.filter(t => t.completed).length;
const total = tasks.length;
const pct = total > 0 ? Math.round(100 * done / total) : 0;
const len = 30;
const filled = total > 0 ? Math.round(len * done / total) : 0;
const bar = "\u2588".repeat(filled) + "\u2591".repeat(len - filled);
dv.paragraph(`**Videos watched**: ${done}/${total} (${pct}%)  \`${bar}\``);
dv.paragraph("See [[01 - Contents]] for the per-domain breakdown.");
```

## Domains
- [[1.0 - General Security Concepts|1.0 — General Security Concepts (12%)]]
- [[2.0 - Threats, Vulnerabilities, and Mitigations|2.0 — Threats, Vulnerabilities, and Mitigations (22%)]]
- [[3.0 - Security Architecture|3.0 — Security Architecture (18%)]]
- [[4.0 - Operations and Incident Response|4.0 — Operations and Incident Response (28%)]]
- [[5.0 - Governance, Risk, and Compliance|5.0 — Governance, Risk, and Compliance (20%)]]

## Schedule

Every study day (Tue Aug 4 – Fri Aug 28) has its own daily note under `Daily Notes/`, with that day's 3 blocks + review block already filled in. Aug 3 is off (a wash day). Open a day via the Calendar plugin (click any date), or jump in directly: [[2026-08-04|Start here — Day 1]]

## Today's tasks

Each block in every daily note is a checkbox task with a due date — this pulls them into one live view.

**Due today:**
```tasks
not done
path includes Daily Notes
due today
```

**Overdue:**
```tasks
not done
path includes Daily Notes
due before today
```

## Weekly board

[[Weekly Board]] — a Kanban view of the same 26 study days, one card per day, dragged through **Backlog → This Week → Today → Done** (with a **Blocked** column for anything a medical appointment knocks loose). A coarser, higher-level view than the Tasks dashboard above — use whichever one actually gets looked at, you don't need both.

## How to track your progress

1. **After you watch a topic's video** → check the box next to it in [[01 - Contents]]. That's the only place "watched" lives — the progress bars above and in Contents read straight off these checkboxes, nothing else to maintain.
2. **After you run practice questions on that topic** → open the note and set `confidence:` to one of:
   - `solid` — got it right, no hesitation
   - `shaky` — got it right but had to think, or half-right
   - `missed` — got it wrong
   Leave `confidence` blank until you've actually tested yourself on it. Blank = not drilled yet.
3. **If `confidence` is `shaky` or `missed`** → write one line in that note's **Practice gaps** section on exactly what tripped you up. Not "missed this" — the actual mix-up, e.g. "mixed up SQL Injection with XSS, forgot SQLi targets the database."
4. **To find what needs work** → use Obsidian's search bar (top left) and type `confidence: missed` or `confidence: shaky`. It searches frontmatter fields without needing any plugin. That list is your review queue.

Do this in order: watch → check the box → drill → tag confidence → fix gap → re-search before the exam. Don't skip step 3 — the tag alone doesn't tell you anything a week from now, the one-line gap note does.

All plugin setup steps are in [[README|README]]. Video sources are in [[References]].
