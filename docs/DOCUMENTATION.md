# Documentation guide

## Purpose

This repository contains the living material of the ROAR community and the documentation describing how the project is shaped. Guild content, event concepts, community-tool designs, and project history should remain distinguishable.

## Status vocabulary

Use these labels whenever the maturity of an idea matters:

| Status | Meaning |
| --- | --- |
| **Established** | Explicitly agreed direction or constraint. |
| **Developing** | Being actively shaped; details may still change. |
| **Proposed** | An option for consideration, not an approved decision. |
| **Open** | No decision has been made. |
| **Temporary** | A current arrangement that is expected or allowed to change. |

A document may contain more than one status. Label individual sections when necessary rather than giving an entire document a misleading status.

## Where information belongs

- Root documents describe the project as a whole.
- docs/ records project decisions, history, documentation rules, and repository structure.
- guild/ contains the guild's working charter, community principles, governance, and activity direction.
- events/ contains event concepts, plans, and records of events that actually take place.
- community-tools/ contains design documentation for Discord bots and other community utilities. It does not imply that the software is implemented.
- operations/ contains practical administrative procedures when they are defined.
- assets/ contains visual and media resources.
- templates/ contains reusable blank documents.

## Source of truth

- Record approved decisions in docs/DECISIONS.md.
- Keep current working guidance in the relevant guild, event, or community-tool document.
- Use ROADMAP.md for future work and CHANGELOG.md for repository changes.
- Use docs/DEVLOG.md for concise human-readable development history.
- If two documents disagree, do not silently choose one. Resolve the conflict and update both.

## Writing and maintenance

- Write clearly and avoid unnecessary jargon.
- Keep public-facing development history in the creative's first-person perspective.
- Distinguish what the creative decided from what AI proposed or implemented.
- Never invent approvals, dates, events, members, roles, or test results.
- Update documents alongside meaningful changes.
- Do not store credentials, private member information, private Discord messages, or sensitive personal records in this public repository.
- For community tools that process member information, document transparency, consent, access, retention, and deletion decisions before describing collection as ready for use.
