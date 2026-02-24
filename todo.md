# Omni-Agent Implementation Workplan

We are following **Path C (Tracer Bullet Approach)** with a global-to-local build order.

## Phase 1: Core Groundwork (COMPLETED)
- [x] Create entire folder structure (Control Tower & Factory Floors).
- [x] Create all placeholder context, memory, and output files.
- [x] Draft global explanation (`explanation.md`).
- [x] Draft master router rules (`gemini-draft.md`).

## Phase 2: Master Controller & Skills (NEXT)
- [ ] Refine `gemini-draft.md` and establish it as the active `GEMINI.md`.
- [ ] Build global shared skills (e.g., Apify scraper patterns, Voice AI endpoints, Web design conventions) in `.agent/skills/`.

## Phase 3: The Integrations & Routing
- [ ] Develop the initial Telegram connection logic.
- [ ] Validate `/prime [pillar]` command to flawlessly switch contexts without bleeding memory.

## Phase 4: System Pros AI (The First Deep Dive)
- [ ] Write `.agent/agents/system-pros.md` (Rules, tone, processes).
- [ ] Fill out `SystemPros/context/` (Current clients, packages, goals).
- [ ] Create automation templates for proposals and Voice AI delivery.
- [ ] End-to-end test System Pros via the Telegram router.

## Phase 5: Skool Mentorship
- [ ] Write `.agent/agents/skool.md`.
- [ ] Migrate/build the Knowledge Base of Q&As.
- [ ] Document GoHighLevel standard operating procedures (SOPs).

## Phase 6: Altus AI (YouTube)
- [ ] Write `.agent/agents/altus-ai.md`.
- [ ] Build research and pipeline workflows.
- [ ] Setup image generation prompts for thumbnails.

## Phase 7: Personal
- [ ] Write `.agent/agents/personal.md`.
- [ ] Connect health, routines, and advisory structures.
