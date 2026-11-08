# Project structure

The repository is organized around the guild's living materials, project history, and practical resources. Add folders when real content requires them; avoid creating empty organizational layers for hypothetical future features.

## Current layout

```text
ROARguild/
├── README.md
├── AGENTS.md
├── CONCEPT.md
├── ROADMAP.md
├── CHANGELOG.md
├── docs/
│   ├── DOCUMENTATION.md
│   ├── DECISIONS.md
│   ├── DEVLOG.md
│   └── PROJECT_STRUCTURE.md
├── guild/
│   ├── README.md
│   ├── CHARTER.md
│   ├── COMMUNITY.md
│   ├── GOVERNANCE.md
│   └── ACTIVITIES.md
├── events/
│   ├── README.md
│   └── sunday-campfires/
│       └── README.md
├── operations/
│   └── README.md
├── assets/
│   └── README.md
└── templates/
    ├── README.md
    ├── event-template.md
    └── meeting-notes-template.md
```

## Folder responsibilities

| Path | Responsibility |
| --- | --- |
| Root | Project entry point, vision, roadmap, contributor rules, and changelog. |
| docs/ | Decisions, development history, documentation standards, and repository map. |
| guild/ | The guild's working charter, community principles, governance, and activity direction. |
| events/ | Event concepts, planning notes, and records of events that actually take place. |
| operations/ | Practical administration and repeatable procedures, once defined. |
| assets/ | Approved visual identity, artwork, banners, and other media. |
| templates/ | Reusable event and meeting documents. |

## File placement rules

- Put a decision in docs/DECISIONS.md, then update the document affected by it.
- Put guild-wide principles in guild/, not in the project development log.
- Give each recurring event series its own folder under events/.
- Keep event proposals visibly separate from confirmed schedules and completed event records.
- Store only public-safe assets and documentation here.
- Do not add member databases, credentials, or private operational records to this public repository.
