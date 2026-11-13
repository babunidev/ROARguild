# Repository instructions for AI and contributors

Follow [the documentation standard](docs/DOCUMENTATION.md) for first-person author voice throughout project documentation, factual changelogs, and naming the AI tool and verified model for each contribution.

## Project identity and scope

- This repository documents ROAR's World of Warcraft Forever community, its guild direction, shared activities, and community-tool concepts.
- ROAR is the wider community/project identity; **Amberhearth is the founded in-game Alliance RP guild**. Do not describe the accepted guild name as undecided.
- The initial community focus is Alliance roleplay in World of Warcraft Forever.
- Target World of Warcraft Forever only. Do not reintroduce Project Epoch, OctoWoW N'Zoth, other clients, or cross-server plans unless the creative explicitly brings them back.
- This repository may contain design documentation for Discord bots and community utilities. Their source code belongs in separate repositories unless explicitly decided otherwise.
- WoW addon source code and addon-specific implementation do not belong here.

## Community identity

- Express the community's values through original, concrete language. Do not publish the former guiding motto as a literal slogan.
- Value companionship, creativity, shared experiences, and belonging over prestige, competition, or rigid expectations.
- Welcome newcomers, returning players, casual players, and roleplayers.
- Do not assume every member wants to roleplay constantly, raid, compete, or follow a fixed progression path.
- Preserve decisions already made: Amberhearth's name and founding, Sunday bonfires as the intended tradition, and Eldgrim's name. Keep individual events, governance powers, and unratified rules clearly marked as planned or proposed.

## Creative authority and attribution

- The human creative owns the vision, priorities, and final decisions.
- AI may research, propose, draft, edit, and implement work when asked.
- Never attribute an original human idea to AI.
- Never describe an AI proposal as accepted until the creative has approved it.
- Never imply that the creative personally performed technical work carried out by AI.
- Public development narratives should use the creative's first-person perspective. Do not begin sentences with "I" or "My". Use "creative", not "creator", for the person making the work.

## Accuracy and project status

Use these status labels consistently:

- **Established** — explicitly agreed direction or constraint.
- **Developing** — actively being shaped, but not finalized.
- **Proposed** — an option awaiting consideration or approval.
- **Open** — no decision has been made.
- **Temporary** — a current arrangement that may change.

Do not turn proposals, assistant suggestions, or historical ideas into settled facts. Preserve uncertainty and record meaningful changes in docs/DECISIONS.md.

For character and story material:
- Preserve established character facts and continuity.
- Distinguish established story canon from new ideas and temporary gameplay details.
- Let stories emerge through gameplay, actions, dialogue, habits, relationships, and small moments.
- Do not invent major character decisions or revelations without direction.

## Reader-first documentation

- Write for a visitor before writing for an agent: begin with what this document is, why it matters, and where to read next.
- Keep current decisions near the top, move historical sequences into dated records, and avoid repeating the same status in every section.
- Use short paragraphs, descriptive headings and Markdown links. Avoid walls of bullets, dense tables and recycled slogans.
- Preserve meaningful facts, attribution, uncertainty and older history; never silently rewrite a past decision as though it had always been settled.

## Documentation workflow

- Read the relevant documentation before making structural or policy changes.
- Keep README.md as the entry point and docs/PROJECT_STRUCTURE.md as the folder map.
- Update the relevant project document whenever an approved decision changes.
- Update CHANGELOG.md for meaningful repository changes.
- Add concise, publication-safe entries to docs/DEVLOG.md for substantial milestones.
- Keep guild content separate from repository/process documentation.
- Keep community-tool design separate from implemented software.
- Do not claim that an event, policy, role, schedule, or feature exists until it has been approved and implemented.
- Do not invent dates, attendance expectations, leadership appointments, member lists, or operational procedures.

## Community tools and privacy

- Use **Eldgrim**, not the retired Oracle working label, for current community-tool and narrative references. The Eldgrim bot, local agent, addon and governance drafts have separate implementation and approval states; check their repository.
- Clearly distinguish intended behavior from implemented and tested behavior.
- Do not commit passwords, tokens, private contact details, member profiles, private Discord messages, or unnecessary personal data.
- Before describing a member-data system as ready for use, document the agreed approach to transparency, consent, access, retention, and deletion. These matters must not be silently assumed.
- Keep public documentation safe for a public repository.

## Change discipline

Prefer small, reviewable changes with clear commit messages. Avoid adding software, automation, workflows, or dependencies unless the project needs them and the creative has approved the direction.
