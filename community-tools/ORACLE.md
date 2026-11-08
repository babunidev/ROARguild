# The Oracle

**Status: Developing concept.**
**Implementation status: Not established by this repository.**

## Overview

The Oracle is a proposed autonomous, AI-driven guild Game Master for the ROAR community. It is imagined as an unusual presence within the guild: a source of stories, quests, recognition, decisions, and shared developments rather than an ordinary chatbot that constantly joins conversations.

The concept combines community awareness with a persistent understanding of members and the guild. It may receive character information from a World of Warcraft addon, learn from Discord community activity, maintain member profiles, and use that context to shape occasional interactions and storylines.

Its final name, personality, voice, and presentation remain open.

## Guiding behavior

The central interaction principle is:

**Observe often. Communicate rarely.**

The Oracle is intended to gather and evaluate context in the background without constantly interrupting members or moderating every conversation.

The current interaction limits discussed are:

- Each player may ask the Oracle one question per day.
- The Oracle sends one guild-wide message per day.
- A daily message may contain a story, quest, recognition of a member, or a plot development.
- The ordinary evaluation and decision cycle happens once per day, when the computer hosting the bot is online.
- Critical situations may justify an exception to the ordinary daily cadence.
- The Oracle should not behave like a constantly active moderator.

These are design requirements under development, not evidence that a bot currently performs them.

## Information sources and processing

The intended system can build its understanding from several sources:

1. **Player registration** — members register their characters so the system can associate later information with the right player and character.
2. **WoW addon data** — a separate addon may provide character information to the bot. The addon itself is outside this repository.
3. **Discord community activity** — guild-channel messages provide social context, shared events, interests, conversations, and other potentially relevant information.

### Daily Discord preparation

The proposed message-processing flow is:

1. Gather new messages from the relevant guild Discord channels since the previous processing run.
2. Summarize those messages into a prepared text before the daily AI run.
3. Give the AI the summary rather than treating every raw message as a separate daily prompt.
4. Identify useful information, keywords, and important details.
5. Associate relevant details with the appropriate member or character.
6. Update the member and guild knowledge stored in the database.

The exact channels, message scope, filtering rules, and treatment of messages that cannot confidently be associated with a member remain to be defined.

## Member profiles and database

The intended design uses an SQL database hosted on the same server as the bot.

Each member is expected to have a profile with four broad areas:

| Profile area | Intended contents |
| --- | --- |
| Character | Registered characters and information supplied by the WoW addon. |
| Social | Relevant interests, conversations, preferences, humor, and connections learned through community interaction. |
| Guild participation | Events, contributions, quests, activities, and other participation context. |
| Personal history | Important memories, accomplishments, relationships, and recorded rewards or disciplinary outcomes. |

The AI is intended to extract keywords and important details and maintain these profiles over time. The precise schema, field definitions, confidence handling, and rules for correcting inaccurate information are not finalized.

This repository describes the intended categories only. Actual member records must never be stored in this public repository.

## Daily presence and communication

The Oracle is intended to have a limited, recognizable presence:

- A member can consult it once per day.
- It contributes one guild-wide message per day.
- It may use that message to introduce a story, offer a quest, recognize a contribution, or advance a plot.
- It can use accumulated character and community context to make those interactions feel connected to the guild's actual experiences.

The Oracle should not fill Discord with constant commentary. Its presence should feel deliberate.

## Delegated authority and decisions

The design discussed gives the Oracle broad delegated autonomy over selected guild systems. The intended authority may include:

- Moderation and muting.
- Rewards and punishments.
- Guild ranks.
- Guild-bank allocation.
- Quests and storylines.

The concept places the Oracle above ordinary guild hierarchy for the responsibilities delegated to it. This is a design direction, not a finalized governance policy or implemented permission set. The relationship between the Oracle and human guild responsibilities still needs to be defined.

### Decision behavior discussed

- Ordinarily, the Oracle should make no more than one decision per day in each relevant category.
- Critical situations may require exceptions.
- It should explain the reasons behind rewards and punishments.
- Positive recognition and rewards are preferred over punishment where appropriate.
- It must not shame players for character race, specialization, talents, or playstyle.
- Racism, sexism, harassment, and bullying are incompatible with the intended community.
- When a dispute requires input, the Oracle may ask the involved people once. If the matter remains undecidable, the discussed concept allows a random or dice-based outcome rather than endless argument.

The precise categories, limits, exception criteria, and decision records remain to be specified.

## Design questions still open

Before implementation, the project still needs to define:

- The Oracle's final name, personality, voice, and in-world presentation.
- Which Discord channels and message types it may observe.
- How members are informed about collection and use of community information.
- What consent is required and whether members can opt out of particular data sources.
- Which profile information members can inspect, correct, or request to have deleted.
- How long summaries, profile details, and decision records are retained.
- How private messages and sensitive information are excluded or handled.
- The exact SQL schema and how uncertain or conflicting information is represented.
- The addon-to-bot communication method and the character fields it supplies.
- What qualifies as a critical situation that can bypass the daily cadence.
- How Oracle decisions are reviewed, corrected, or appealed.
- How its delegated authority interacts with human leadership and guild governance.
- What happens when the host computer is offline and a daily run is missed.

These are open design questions, not existing policies. They must be resolved before the corresponding behavior is presented as operational.

## Scope and implementation boundary

This document records the Oracle's current design direction. It does not describe a completed architecture, working integration, tested database, or deployed bot.

The Oracle is a ROAR community-tool concept. Its implementation may be developed in a separate repository. Any WoW addon that supplies character information also remains a separate project.
