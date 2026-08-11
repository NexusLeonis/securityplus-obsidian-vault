# Security+ (SY0-701) — Home

Study vault for the CompTIA Security+ SY0-701 certification, organized around the official CompTIA objectives and Professor Messer's course order.

## Start here

- [[00 - CompTIA Objectives Summary]] — official exam scope and weighting
- [[01 - Contents]] — all 120 Messer topics in course-note/video order

## Overall learning progress

```dataviewjs
const contents = dv.page("01 - Contents.md");
const tasks = contents.file.tasks;
const done = tasks.filter(t => t.completed).length;
const total = tasks.length;
const pct = total > 0 ? Math.round(100 * done / total) : 0;
const len = 30;
const filled = total > 0 ? Math.round(len * done / total) : 0;
const bar = "\u2588".repeat(filled) + "\u2591".repeat(len - filled);
dv.paragraph(`**Learning loops complete**: ${done}/${total} (${pct}%)  \`${bar}\``);
dv.paragraph("See [[01 - Contents]] for the per-domain breakdown.");
```

## Domains

- [[1.0 - General Security Concepts|1.0 — General Security Concepts (12%)]]
- [[2.0 - Threats, Vulnerabilities, and Mitigations|2.0 — Threats, Vulnerabilities, and Mitigations (22%)]]
- [[3.0 - Security Architecture|3.0 — Security Architecture (18%)]]
- [[4.0 - Operations and Incident Response|4.0 — Security Operations (28%)]]
- [[5.0 - Governance, Risk, and Compliance|5.0 — Security Program Management and Oversight (20%)]]

## 60-day schedule

**Tue Aug 11 – Fri Oct 9**

- **Aug 11 – Sep 21:** 30 weekday learning days, 4 Messer topics per day
- **Sep 22 – Oct 9:** 14 weekday practice/repair days
- **Weekends:** recovery or catch-up; no new scheduled content

Start here: [[2026-08-11|Day 1 — Tue Aug 11]]

## Today's tasks

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

## Tracking

1. Finish a topic's Messer-notes → one-video-pass → recall loop, then check it in [[01 - Contents]].
2. During Aug 11–Sep 21, leave `confidence:` blank; use closed-note recall to learn the material.
3. Starting Sep 22, set `confidence:` to `solid`, `shaky`, or `missed` after quiz/practice questions.
4. For `shaky` or `missed`, write the exact mix-up in **Practice gaps**, then search those fields to build the repair queue.

Your original Aug 4–10 daily notes can stay as the record of the first attempt. The 60-day restart begins Aug 11.
