# Development log

A concise account of meaningful moments in the making of ROARguild. Entries are written from the human creative's perspective and distinguish direction from implementation.

## 2026-11-08 — Defining the Oracle's operating model

The latest design discussion clarified what I want the Oracle to become: not a conventional chatbot, but an autonomous supernatural Guild Game Master with a place in the guild's stories and delegated responsibility for selected community systems.

The intended guild model has no human guild master. Members remain equal to one another, while ranks represent social standing and recognition. The Oracle makes its own decisions within its delegated scope. A trusted committee handles the practical guild bank work, carrying out the Oracle's allocations rather than approving them.

The technical shape is now clearer as well. The Discord bot and SQL database stay online on the server, while the AI agent runs on my computer approximately once a day and shuts down after its work. The bot collects Discord activity and other inputs; the local agent interprets them, updates persistent character sheets with keywords rather than copied conversation excerpts, evaluates the guild, and acts through the bot.

The concept now also includes a private 0–100 standing score, daily individual questions and guild proclamations, a limited role in the Sunday bonfire gathering, personalized fire-themed quests, screenshot-and-witness verification, freely chosen rewards, daily guild bank snapshots, and autonomous graduated moderation.

One important boundary remains explicit: raw Discord logs may be collected for processing, but their access, retention, deletion, consent, and the wider member-data policy have not been settled. The Oracle's long-term character sheets are intended to preserve interpretations, not conversation transcripts.

The aim is the full vision, built incrementally rather than reduced to a separate MVP. These are design requirements, not implemented or tested features.

## 2026-11-08 — Giving the project a home

The repository began as an empty public project. With the initial Alliance roleplaying direction in mind, I asked AI to establish a documentation system that could hold the guild's concept, decisions, practical materials, and history without pretending every idea was already settled.

The first structure separated the guild's living documents from project history and working rules. ROAR remained the repository identity, while Amberhearth and the Sunday bonfire concept were recorded as developing ideas rather than decisions.

## 2026-11-08 — Bringing the wider vision into the documentation

The project conversations clarified that ROAR is about more than forming a guild. The community is meant to be a welcoming fellowship built around shared experiences, creativity, and companionship in Azeroth. Character stories, small everyday moments, and unhurried gatherings belong alongside traditional group content.

The traveling-hearth idea became more specific: a possible Sunday gathering that moves through Alliance regions, lighting fires along roads and paths for travelers to meet, share stories, and sing. It remains a concept rather than a published schedule.

The Oracle also emerged as a substantial community-tool design. Its intended role, Discord information flow, member-profile categories, daily communication limits, and delegated authority are now documented separately. The document records design intent, not completed software.

These updates curate the direction discussed so far. They do not finalize the guild name, adopt the charter, establish governance, schedule an event, or claim that the Oracle has been implemented.
