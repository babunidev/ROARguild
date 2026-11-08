# Project structure

The repository is organized around the community's living materials, project history, and practical resources. Add folders when real content requires them; avoid creating empty organizational layers for hypothetical future features.

## Current layout

- Root: README.md, AGENTS.md, CONCEPT.md, ROADMAP.md, CHANGELOG.md
- docs/: DOCUMENTATION.md, DECISIONS.md, DEVLOG.md, PROJECT_STRUCTURE.md
- guild/: README.md, CHARTER.md, COMMUNITY.md, GOVERNANCE.md, ACTIVITIES.md
- events/: README.md and one folder per recurring event concept or series
- community-tools/: README.md and design documents for community utilities
- operations/: practical guild administration, once procedures are defined
- assets/: approved public-safe visual and media resources
- templates/: reusable event and meeting documents

## Folder responsibilities

| Path | Responsibility |
| --- | --- |
| Root | Project entry point, vision, roadmap, contributor rules, and changelog. |
| docs/ | Decisions, development history, documentation standards, and repository map. |
| guild/ | The guild's working charter, community principles, governance, and activity direction. |
| events/ | Event concepts, planning notes, and records of events that actually take place. |
| community-tools/ | Design intent and requirements for Discord bots and community utilities. |
| operations/ | Practical administration and repeatable procedures, once defined. |
| assets/ | Approved visual identity, artwork, banners, and other media. |
| templates/ | Reusable event and meeting documents. |

## File placement rules

- Put an approved decision in docs/DECISIONS.md, then update the document affected by it.
- Put guild-wide principles in guild/, not in the project development log.
- Give each recurring event series its own folder under events/.
- Keep event proposals visibly separate from confirmed schedules and completed event records.
- Put community utility design notes in community-tools/; keep actual source code in its own repository unless explicitly decided otherwise.
- Store only public-safe assets and documentation here.
- Do not add member databases, credentials, private messages, or private operational records to this public repository.
