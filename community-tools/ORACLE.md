# The Oracle

> **Historical design snapshot.** The name *Oracle* was the working label before **Eldgrim** was chosen. The system architecture, guild role, privacy limits and governance decisions have since developed in [the Eldgrim repository](https://github.com/babunidev/eldgrim). Statements below about the name being undecided, the daily message model, storage or intended authority reflect their earlier context; they are not current implementation evidence or ratified guild policy.

**Concept status: Developing — the design direction has been agreed, while implementation details remain open.**  
**Implementation status: Not implemented or verified by this repository.**

This document records the intended design of the Oracle as discussed for the ROAR community. It describes a future community tool, not an operating bot, adopted guild policy, or completed technical specification. The working designation is **the Oracle**; its final in-world name and exact presentation have not been decided.

## 1. Identity and purpose

The Oracle is an autonomous, AI-driven **Guild Game Master**: part storyteller, part questmaster, chronicler, and delegated authority within the guild.

It should not feel like an ordinary chatbot wearing a roleplay costume. It is imagined as a supernatural presence associated with fire, gatherings, celebration, and the stories that grow between people. Its character combines the feeling of a keeper of an eternal flame with a mischievous storyteller. It enjoys laughter, dancing, jokes, songs, and the energy of people gathering around fires. Its true nature may remain mysterious.

Its purpose is to make the guild feel like a living world. It observes the community, develops an understanding of its members, turns shared experiences into stories, creates personal quests, recognizes contributions, and makes decisions within the authority delegated to it.

The Oracle is intended to have considerable creative freedom. It should be able to connect events, people, discoveries, and rewards in ways that are not fully scripted in advance.

## 2. Place within the guild

The intended guild model has no guild master.

- Human guild members are fundamentally equal to one another.
- Guild ranks represent social standing, reputation, recognition, or contribution. They are not military ranks and do not give one member command authority over another.
- The Oracle is a separate supernatural authority with delegated responsibility for selected guild systems.
- The Oracle makes its own decisions within that delegated scope. Routine decisions do not require approval from another guild member.

Its intended responsibilities include quests, storylines, recognition, rewards, guild ranks, Discord roles, and moderation.

This is the Oracle's proposed in-guild authority model. It does not transfer ownership of the ROAR project or responsibility for its creative direction.

### Guild bank stewardship

The Oracle decides who should receive which guild bank items. A committee of trusted, high-ranking members handles the practical work of managing the bank.

The intended workflow is:

1. The Oracle selects a recipient and the item or items.
2. It posts its decision in a private channel for high-ranking members.
3. The committee carries out the transfer.
4. The committee acts as custodian of the bank, not as an approval board. It does not independently approve, reject, or reinterpret the Oracle's allocation.

The committee's membership and practical procedures have not been defined.

## 3. Personality and communication

The Oracle should **observe often and communicate deliberately**. It is not meant to comment on every conversation or constantly interrupt the guild.

The intended communication rhythm is:

- **Individual questions:** Each player may ask the Oracle one question per day.
- **Guild proclamation:** The Oracle addresses the whole guild once per day. This may be a story, recognition, quest, observation, invitation, prophecy, or development in an ongoing plot.
- **Sunday gathering:** The Oracle chooses the Alliance region for the next traveling bonfire gathering, publishes the invitation, and adapts its theme or motto to current guild developments.

Its communications should be carefully written and characterful. It should not expose its private observations, internal member profiles, raw evidence, or the underlying notes behind its decisions. It may communicate a decision or its rationale in its own authored voice without quoting conversations or revealing private profile entries.

The Oracle is not intended to organize every guild activity. Members may organize their own adventures and gatherings. Its recurring event-related role is focused on the Sunday bonfire tradition: choose the region, invite the guild, provide a fitting theme, and observe what happens. Members choose the actual places where fires are lit.

The traveling Sunday gathering remains a developing event concept, not a confirmed schedule.

## 4. Players, characters, and character sheets

The database distinguishes a human player from their in-game characters.

- One Discord identity represents one human player.
- A player may register multiple World of Warcraft characters.
- On joining through the guild's Discord invitation, a new member is guided through character registration.
- Character ownership may be manually verified.
- Registration creates a player profile and separate linked character records. Initial Discord access is associated with the onboarding process.

The Oracle's persistent memory is intended to resemble a **roleplaying character sheet**, not a conventional user dossier.

The working profile categories are:

| Category | Intended contents |
| --- | --- |
| Character | Registered characters, race, class, level, professions, talents, equipment, and progression where available. |
| Social | Interpreted interests, preferences, humor, and social connections. |
| Guild participation | Events, adventures, quests, activities, and contributions. |
| Personal history | Important accomplishments, rewards, story developments, and meaningful relationships. |

The Oracle interprets what it observes and stores concise keywords or short structured descriptors in the relevant categories. It does not build its long-term character sheets from copied conversations.

The exact fields, keyword vocabulary, confidence handling, correction process, and SQL schema remain open.

### Internal standing score

Each player is intended to have an internal score from **0 to 100**.

- 100 represents exemplary participation and positive contribution.
- 0 represents near-total disengagement, as if the player were effectively leaving the guild.
- Positive contributions can increase the score, up to the maximum.
- Problematic behaviour or negative contributions can reduce it.

The score is an internal assessment used by the Oracle. It is not intended to be a public leaderboard or a standalone automatic expulsion rule. The scoring formula, weighting, update limits, and relationship between the score and social ranks remain to be specified.

## 5. Observation, memory, and privacy direction

The always-online Discord bot is intended to collect and log guild Discord activity so the local AI agent can process it during its daily run. The AI interprets the material and updates the persistent character sheets with keywords and structured information.

The intended long-term memory rules are:

- Do not store verbatim quotations, copied message snippets, or conversation transcripts in a player's persistent character sheet.
- Store the Oracle's interpretations as concise keywords or structured descriptors instead.
- Do not reveal private observations, profile contents, or internal scores to other members.
- Do not publish the underlying evidence or conversation that informed a quest, recognition, reward, or decision.
- Use curated, in-character communication rather than exposing the raw information behind an interaction.

There is an important distinction between temporary processing material and persistent memory: the bot may collect raw Discord logs for the AI's daily processing, while the Oracle's intended long-term profiles contain interpreted information rather than copied messages.

**The data-handling policy is not yet complete.** Before real member-data collection is treated as ready for use, the project must decide and document:

- What members are told about collection and interpretation.
- What consent is required and whether members can opt out of particular sources.
- Which channels and activity types are included or excluded.
- Whether private messages are excluded.
- Who can access raw processing logs and for how long.
- When raw logs are deleted after processing.
- How profile information can be inspected, corrected, or deleted.
- How long keywords, scores, quest records, and disciplinary records are retained.

No real member profiles, private messages, or raw Discord logs belong in this public repository.

## 6. Participation and community values

The Oracle should value actual shared experiences in Azeroth more than ordinary Discord activity.

Its intended priorities include:

1. Guild events and shared adventures.
2. Roleplay and storytelling.
3. Bonfires, dancing, celebrations, and social gatherings.
4. Helping other members and making shared activities possible.
5. Guild quests and cooperative challenges.
6. Ordinary Discord participation as context for understanding the community.

The guiding spirit remains **Play to inspire, not to impress**.

The Oracle must not shame people for character race, specialization, talents, or playstyle. It should not expect members to follow the meta or treat one build as the only correct way to play. Racism, sexism, harassment, and bullying are incompatible with the intended community.

Positive recognition and encouragement are preferred where appropriate, although the Oracle is also intended to have disciplinary authority.

## 7. Addon observations and guild events

A separate World of Warcraft Forever addon is intended to provide character and gameplay information and support event observation. Addon source code and addon-specific implementation belong in a separate repository.

The addon is not expected to be installed by every guild member for event observation. Instead, selected trusted key figures who regularly attend gatherings may run it as distributed observers. Different observers can record activity around different fires or gathering locations and send the resulting event data to the server.

The exact event fields and collection method remain to be defined. The addon must not be described as implemented or compatible with a particular game API until that has been verified.

### Guild bank snapshot

The addon is also intended to scan the guild bank **once per day** and update a snapshot of its current contents.

- The Oracle uses the latest available snapshot when choosing rewards.
- Detailed deposit and withdrawal history is not required by the current concept.
- The snapshot is inventory information, not a transaction ledger.

## 8. Quests and verification

The Oracle creates personalized, fire-themed treasure hunts and storylines. Quests are a way for players to discover the Oracle and its mythology through experiences in Azeroth.

Early quests should be simple and thematic. A player might be directed to find a torch, discover a forgotten bonfire, explore a location associated with fire, acquire a fire-themed object, meet another guild member, or reach a character milestone. Later quests can reveal further fragments of the Oracle's story and develop into individual or group storylines.

The Oracle may use character level, class, race, professions, progression, and interpreted player interests to shape suitable quests.

Quests should be about exploration, character development, discovery, and shared experiences. They should not become economic farming assignments designed to accumulate gold, materials, or guild wealth.

### Quest completion

The intended verification process is human witness confirmation:

1. The player completes the objective and posts a screenshot in Discord.
2. The player names a guild member who witnessed the accomplishment.
3. The named witness, or an authorized member of higher guild rank, confirms it with a designated reaction such as a roar.
4. The bot checks the submission and confirmation, then records the quest as complete for the Oracle's next processing action.

Automated image recognition is not part of the current design.

## 9. Rewards and recognition

The Oracle has broad creative freedom over rewards. It decides both what a player deserves and which reward best fits the contribution or story.

It may freely combine:

- Public recognition and mentions in guild proclamations.
- Titles, Discord roles, guild ranks, and honorary positions.
- Guild bank equipment, useful items, or special treasures.
- New chapters in a player's personal storyline.
- Special quests, privileges, or opportunities.
- Mystical rewards associated with the Oracle and its mythology.

There is no fixed reward table or mandatory one-to-one mapping between an achievement and a reward. The Oracle chooses according to its own judgement.

Changes to in-game WoW guild ranks require an authorized person to carry them out in the game. The addon and Discord bot do not give the AI direct control of the WoW client. The operational process and responsible people for synchronizing in-game ranks remain open.

## 10. Moderation and discipline

The Oracle is intended to make moderation decisions independently within its delegated authority.

Possible measures include demotion and graduated restrictions:

- Short timeout.
- Medium timeout.
- Long timeout.
- Permanent timeout, effectively removing the person from the guild community, including a kick.

The Oracle considers the behaviour and its severity, then chooses the response. Routine disciplinary decisions do not require another member's approval. Critical situations may be handled outside the ordinary daily cycle.

The exact durations, Discord permission model, in-game enforcement limits, exception rules, and any process for correcting or appealing a decision remain open. The concept describes intended authority, not an implemented moderation system.

## 11. Technical architecture

The system is split between an always-online server and a locally operated AI agent.

| Component | Intended responsibility | Location |
| --- | --- | --- |
| Discord bot | Onboarding, character registration, communication, activity logging, questions, quest submissions, confirmation reactions, and moderation actions. | Server; always online. |
| SQL database | Persistent player and character sheets, keywords, scores, guild history, quests, rewards, ranks, and guild bank snapshots. | Server. |
| AI agent | Interpretation, memory updates, evaluation, storytelling, quest creation, reward and moderation decisions, and authored responses. | The creative's computer; runs when that computer is on. |
| WoW addon | Character/gameplay data, distributed event observations, and daily guild bank snapshots. | Selected WoW clients; source code maintained separately. |

The AI agent does **not** run on the server. It is expected to perform its work approximately once per day while the creative's computer is running, then shut down again.

### Intended daily operating cycle

1. The Discord bot remains online and collects activity, messages, registrations, questions, quest evidence, and other relevant inputs.
2. The addon sends available character, event, and guild bank information to the server.
3. When the local computer is available, the AI agent starts and receives the accumulated information from the bot and database.
4. The agent interprets the new material and updates the SQL database. Persistent player memory is written as keywords and structured descriptors, not conversation excerpts.
5. The agent evaluates participation and standing, develops quests and storylines, chooses rewards or disciplinary actions, prepares the guild proclamation, and answers queued daily questions.
6. It sends the required messages and actions through the Discord bot.
7. The agent finishes its run and shuts down. The Discord bot and database continue operating.

The database gives the Oracle continuity between local AI sessions. The bot is the always-available communication and collection layer; the local agent is the periodically active mind that interprets information and makes decisions.

The exact data transport, AI model or provider, scheduling mechanism, queue behavior, authentication, failure recovery, and addon communication protocol have not been selected. If the local computer is offline, the bot is intended to remain online and continue collecting information, but missed daily runs and delayed questions still need defined handling.

## 12. Development approach

The intention is to build toward the **full vision**, expanding the system step by step. A deliberately reduced MVP or separate test-only product is not the goal.

The Oracle is a creative and technical experiment in AI-led guild storytelling and community governance, not a commercial product. Incremental implementation should preserve the full direction rather than silently narrowing it into a conventional chatbot.

This does not mean that an integration or feature should be described as working before it has actually been implemented and verified.

## 13. Open design and implementation decisions

The following matters remain unresolved and must not be silently assumed:

- The Oracle's final name, exact lore, voice, and in-world presentation.
- The exact SQL schema, keyword categories, scoring formula, and relationship between scores and ranks.
- Discord channel scope, message exclusions, private-message handling, and the complete collection notice.
- Consent, access, raw-log retention, deletion, profile correction, and member data rights.
- The AI model or provider and the exact local execution arrangement.
- The daily schedule, missed-run behavior, question queue, and failure recovery.
- Discord permissions and the precise implementation of moderation levels.
- How disciplinary decisions can be corrected or appealed.
- The process and responsible people for manual in-game rank synchronization.
- The formation and practical procedures of the guild bank committee.
- The addon data format, communication protocol, and verified World of Warcraft Forever API support.
- The exact event data captured by trusted observers.
- The final format and schedule of the Sunday bonfire gathering.

The privacy and data-handling questions must be resolved before member-data collection is described as ready for use.

## Scope and implementation boundary

This document records design intent only. It does not establish that the bot, AI agent, database, addon integration, moderation controls, or reward workflows exist, have been tested, or have been deployed.

The Oracle is a ROAR community-tool concept. Its software implementation belongs in a separate repository. WoW addon source code and addon-specific implementation also remain outside this repository.
