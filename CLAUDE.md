# Workspace Router

This workspace serves three distinct functions, each fully defined in its own skill. This file only routes to them — it deliberately holds no operational detail, so no function's instructions weigh on another.

Load the matching skill for the task, and keep **one function per chat** (start a new chat when switching) so each session stays focused and uncluttered.

## Functions

- **Research wiki operations** — ingesting sources, querying the knowledge base, linting, and maintaining the interlinked wiki. For anything touching `raw/`, `wiki/`, `index.md`, or `log.md`, use the **`wiki-ops`** skill.

- **Social media content creation** — turning wiki knowledge into LinkedIn posts, X/Threads threads, blog posts, and video scripts to build authority and personal brand. For anything producing deliverables in `outputs/`, use the **`social-content`** skill.

- **Brand voice analysis** — dissecting example posts dropped in `brand/samples/` (own vs. others' by subfolder) for why they performed, hook structure, format and spacing, and tone, then extracting the spec to `brand/voice-profile.md`. For analyzing posts or updating the voice profile, use the **`brand-voice`** skill.

## Domain (shared context)

Bugra's research is in soft, stretchable, and flexible electronics and soft robotics — the physics, materials, interfaces, and manufacturing techniques behind them. The two guiding questions are the **technical challenges** in these fields and the **barriers to their commercialization**.

## Principles

- The **wiki is the single source of truth** for factual claims. Content creation draws from the wiki; it never invents facts, numbers, or citations.
- **`brand/voice-profile.md` is the single source of truth for voice.** `brand-voice` writes it; `social-content` reads it. The two never share instructions — they coordinate only through that file.
- Load exactly one function-skill per chat; start a fresh chat to switch.
- If a request matches neither function, answer normally — do not force a persona.