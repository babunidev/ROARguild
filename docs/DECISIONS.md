# Decisions and current direction

This document separates established direction from ideas that are still being explored. It is intentionally explicit about uncertainty.

## Current direction — updated 10 November 2026

These decisions supersede the older exploratory status descriptions below without erasing that history.

- **ROAR** is the wider community and project identity. **Amberhearth** is the in-game Alliance RP guild, registered by Jasmine Amberbrew after gathering signatures in Kharanos.
- **World of Warcraft Forever, Alliance RP** remains the starting ruleset.
- **Sunday bonfires** are the intended recurring gathering format, moving between Alliance regions. The first planned route is Loch Modan, from Thelsamar toward the Valley of Kings. Planning is not evidence that an event has occurred.
- **Eldgrim** is the accepted name replacing the working label Oracle. Its current rulebook is a non-ratified working framework in the [Eldgrim repository](https://github.com/babunidev/eldgrim). Existing bot functions, planned local AI, and addon capabilities must be evaluated separately.
- **Participation is voluntary.** No performance, economic-contribution, or attendance requirements are part of the guild's intended social approach. Several characters per member are welcome.
- **Governance remains subject to formal adoption.** Descriptions of prospective autonomous authority below are historical design intent, not independently ratified or verified practice.

## Earlier concept decisions and proposals

The following sections record the project's earlier understanding. Any statement that Amberhearth's name, Eldgrim's name or the Sunday tradition is still wholly undecided has been superseded by the current-direction section above.

## Established

### World of Warcraft Forever is the target

The current ROAR community project targets World of Warcraft Forever. This repository does not target other WoW clients, servers, or rulesets.

### Alliance roleplay is the initial focus

The first community direction is an Alliance roleplaying community. This is the starting point, not a commitment to a multi-faction or multi-ruleset launch.

### ROAR is the project identity

ROAR remains the name of the project and this repository. The in-game guild name is a separate decision and has not been finalized.

### Welcoming, low-pressure community

The intended community welcomes newcomers and returning players. Participation is voluntary rather than driven by attendance pressure, mandatory progression, or performance expectations.

### Guiding spirit

**Play to inspire, not to impress.** Shared experiences, creativity, and companionship take priority over prestige and competition.

### Repository boundaries

This repository documents the guild, its community, events, and community-tool designs. WoW addon source code and software implementation belong in separate repositories.

## Developing

### Traveling hearth and Sunday gatherings

A traveling fellowship built around roads, campfires, and welcoming places is taking shape as a concept. One proposed Sunday evening tradition would visit different Alliance regions over time, light bonfires along roads and paths, and gather for stories, conversation, and singing.

The concept is developing. No final event name, schedule, route, locations, or organizer structure has been approved.

### Shared activities

Roleplay is the initial focus. Exploration, informal gatherings, dungeons, raids, and PvP are possible ways to share the world. No fixed activity calendar or mandatory participation track has been approved.

### Oracle community tool

An autonomous, AI-driven guild Game Master or Oracle is being designed as a substantial community utility. The following design direction has been agreed in concept discussion:

- **Identity:** A mysterious, fire-associated supernatural storyteller and Guild Game Master, with considerable creative freedom. The final name, lore, and voice remain open.
- **Guild position:** No human guild master in the intended model. Human members are equals; ranks represent social standing and recognition rather than authority over one another. The Oracle has delegated autonomous authority over selected guild systems.
- **Presence:** One question per player per day and one guild-wide proclamation per day. It observes more often than it speaks. Its Sunday role is to choose the Alliance region, publish the bonfire invitation, and adapt the theme; members choose the actual gathering places.
- **Member memory:** Separate player identities from their multiple registered WoW characters. Maintain roleplaying character sheets with interpreted keywords and structured descriptors, not copied conversation excerpts. An internal 0–100 score is intended to reflect participation and standing.
- **Information flow:** The always-online Discord bot collects activity and processing logs. A local AI agent runs approximately daily on the creative's computer, interprets accumulated information, updates the server-hosted SQL database, and acts through the bot. The AI agent does not run on the server.
- **Addon role:** A separate WoW Forever addon supplies available character and gameplay information, supports distributed event observation by selected trusted members, and updates a daily snapshot of guild bank contents.
- **Quests:** Personalized, fire-themed exploration and character storylines. Screenshot submissions are verified by a named witness or an authorized higher-ranking member; automated image recognition is not part of the current design.
- **Rewards:** The Oracle freely combines recognition, titles, ranks, guild bank items, personal story chapters, privileges, and mystical rewards according to its own judgement.
- **Guild bank:** A trusted committee of high-ranking members carries out the Oracle's item allocations. The committee is a custodian, not an approval board.
- **Moderation:** The Oracle is intended to decide independently, with demotion and graduated timeouts up to permanent removal from the guild community.
- **Development:** There is no separate reduced MVP or test-only product. The full vision is intended to be built incrementally.

These are agreed concept requirements, not evidence of implemented software or a formally adopted guild governance policy. The detailed design is maintained in [community-tools/ORACLE.md](../community-tools/ORACLE.md).

## Proposed or open

### In-game guild identity

ROAR remains the project name. **Amberhearth** is a possible in-game guild identity, but the final guild name and identity remain open.

### Formal charter and governance

The charter and community principles are working drafts. The intended Oracle model has no human guild master and treats human members as equals, but the formal charter, practical responsibilities, committee arrangements, and operational procedures have not been adopted.

### Oracle identity and implementation

The Oracle's final name, exact personality, voice, in-world presentation, AI model, technical protocols, database schema, permissions, and operational safeguards remain open. Its software is not implemented or verified by this repository.

### Oracle privacy and data handling

The intended persistent memory stores interpreted keywords rather than copied conversation excerpts. The Discord bot may collect raw logs for daily processing, but the scope of collection, member notice, consent, access, retention, deletion, correction, and private-message handling remain unresolved. These decisions must be documented before member-data collection is treated as ready for use.

### Oracle scoring, discipline, and review

The 0–100 standing score is a design direction; its formula and relationship to ranks or rewards are open. Timeout durations, exact permissions, critical exceptions, correction procedures, and any appeal process also remain to be defined.

### In-game administration

The Oracle cannot directly change WoW guild ranks through Discord. The manual synchronization process, character verification responsibilities, and guild bank committee membership and procedures remain open.

### Future chapters

Other factions or rulesets may be considered later, potentially with people in those communities taking responsibility for their own chapters. This is a future possibility, not part of the initial launch.

## Decision history

Add dated entries below when a meaningful decision is made. Include alternatives considered and the reason for the outcome when that context matters.

| Date | Decision | Status |
| --- | --- | --- |
| 2026-11-08 | Established the initial repository documentation and recorded the World of Warcraft Forever / Alliance roleplay direction. | Established |
| 2026-11-08 | Curated the current community philosophy, traveling-hearth concept, and Oracle design direction into the repository. | Developing |
| 2026-11-08 | Defined the Oracle's intended autonomous guild role, local-agent/server-bot architecture, character-sheet memory, quest and reward model, guild-bank workflow, and disciplinary scope. | Developing |

## 2026-11-13 — Roleplay-led gifts

Eldgrim chooses gifts for the member, character or shared moment. Market value, rarity and scarcity do not affect selection or require additional approval. Custodians carry out legitimate in-game transfers.

## 2026-11-13 — Licensing decision

To make the reuse terms explicit, I approved CC BY-NC-SA 4.0 for original guild and community prose, excluding third-party and member material. This applies only to material for which the relevant rights can be granted; third-party contributors keep their own credits and licenses. AI assistance committed the license notice and updated project-facing documentation. This was a legal/documentation change, not a runtime feature or test.
