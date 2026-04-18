# VulcanX Champion — MVP

Live demo: **https://jamie323.github.io/vulcanx-champion-mvp/**

A prototype of the **Champion / Companion system** for VulcanX.

Each user raises a single fantasy creature from a newly-hatched whelp (Level 1) to a legendary warlord (Level 50) through continued activity on the platform. The same individual grows visibly across 50 levels — identity preserved, power progression earned, environment evolves from nursery to myth.

## What's in the demo

- **9 anchor illustrations** spanning Level 1 → Level 50 of a single orc (Grokk Ironfang)
- **Drag the level slider** from 1 to 50 — title, zone, stats, stage badge, and artwork all update
- **6-trait stat system** (Strength, Vitality, Agility, Ferocity, Intelligence, Luck)
- **Potion buttons** with diminishing-returns curve (+10 per potion up to 10 spent, then +5, then +2, then +1)
- **Hard stage caps** — stats can't overflow their stage, protecting game balance
- **Evolution panel** that lights up when 2 traits pass 60% of cap; click to advance stage (consumes 1 Evolution Potion)
- **Legendary aura** effect on Level 50

## Stages (per species)

| Level band | Stage | Zone |
|---|---|---|
| 1–4 | Whelp | Nursery |
| 5–9 | Pup | Tribe |
| 10–14 | Adolescent | Tribe |
| 15–19 | Warrior | Camp |
| 20–29 | Champion | Camp |
| 30–39 | Elite | War |
| 40–44 | Warlord | War |
| 45–49 | Ascendant | Myth |
| 50 | **Legendary** | Myth |

## Production cost for this prototype

Entire 50-stage visual library generated for **~$0.88** in API credits. Pipeline: Flux 1.1 Pro (anchor) + Flux Kontext Pro (identity-preserving chain to other stages) via Replicate. Full production notes in `SPEC_CHAMPIONS.md` in the private PoC repo.

## What this is NOT (yet)

- Not wired to a backend — state is in-browser only
- No real combat or expedition system
- No NFT / on-chain integration
- Only one species (orc) — elf/demon/dragon/goblin planned next

## Roadmap

1. ✅ 1-species evolution proof
2. 🔲 10-person blind test — "do these 9 images read as the same orc growing up?"
3. 🔲 Species 2 (elf)
4. 🔲 Idle XP timer (first retention loop)
5. 🔲 Stat card / Top Trumps compare mode
6. 🔲 Async stat battler
7. 🔲 Auto-battler combat

## Credits

AI image generation: `black-forest-labs/flux-1.1-pro` and `black-forest-labs/flux-kontext-pro` via Replicate.
