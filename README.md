# One Good Icon

![One Good Icon logo](assets/one-good-icon-lockup.png)

> Explore many. Ship one good icon.

One Good Icon is an agent skill for the complete app-icon cycle: divergent exploration from real product material, specialist critique at real sizes and in context, then platform-ready delivery for Apple, Android, and Expo.

## What makes it different

- **Real material first.** Product, UI, brand, screenshots, sketches, references, existing icons, and selected generations are first-class inputs.
- **Three human-gated phases.** Explore → Refine → Ship. A generated favorite is not silently promoted into production.
- **Native visual exploration.** The agent uses its host's image generator when available, with portable prompts as the fallback.
- **Concrete criticism.** It diagnoses visible failures instead of inventing a score.
- **Representation follows the artwork.** Vector reconstruction, raster masters, and layered Icon Composer sources are choices, not dogma.
- **Self-contained workflow.** One Good Icon replaces external icon-generation skills and API-backed CLIs; MAYA, Taste, Impeccable, or prototype can still offer an optional second opinion.

## Install

Install from GitHub with the [Skills CLI](https://github.com/vercel-labs/skills):

```bash
npx skills add florianrumigny/one-good-icon-skill
```

The CLI detects supported agents and lets you choose where to install the skill. To install it globally for Codex without prompts:

```bash
npx skills add florianrumigny/one-good-icon-skill \
  --skill one-good-icon \
  --global \
  --agent codex \
  --yes
```

Verify the installation with:

```bash
npx skills ls --global --agent codex
```

Then start a new Codex task and invoke `$one-good-icon`.

## Use cases

Give the skill the real product material you have and tell it how far to go. It pauses for human selection between Explore, Refine, and Ship.

**Start from an idea**

> Use `$one-good-icon` to explore an app icon for a calm shared grocery-list app. Create 4–6 genuinely different directions and stop after the exploration board.

**Derive an icon from an existing product**

> Use `$one-good-icon` with this product brief, UI screenshots, brand palette, and visual references. Extract the visual principles worth preserving without copying proprietary elements, then explore icon directions.

**Improve an existing icon**

> Use `$one-good-icon` to critique this current icon at 1024, 256, 128, 64, and 32 px. Diagnose concrete recognition, silhouette, contrast, distinctiveness, and platform-resilience problems, then propose targeted variations.

**Refine selected candidates**

> Use `$one-good-icon` to refine candidates B and D. Test them on light, dark, and busy backgrounds, in a homescreen grid, and across relevant iOS and Android masks. Stop for my approval before Ship.

**Ship platform assets**

> Use `$one-good-icon` to ship this approved icon for my Expo project. Preserve the selected master, choose raster, vector, or useful layers based on the artwork, generate the iOS and Android assets, update the project configuration, and verify the final files and renders.

**Use it with MAYA**

> Let `$maya` own the broader art direction and `$one-good-icon` own the specialist app-icon workflow. Explore from the attached product material and stop when a human choice is required.

## Companion: MAYA

[MAYA](https://github.com/florianrumigny/maya) can own the wider product art direction, visual exploration, and global critique while One Good Icon owns the specialist app-icon workflow. This integration is optional; One Good Icon works on its own.

## Repository map

```text
SKILL.md                 compact workflow and routing
agents/openai.yaml       Codex-facing metadata
assets/                  logo lockup and skill-avatar marks
references/explore.md    divergence and reference handling
references/refine.md     variation and test protocol
references/critic.md     specialist review lens
references/ship.md       production decision and final verification
references/apple.md      Apple/Icon Composer adapter
references/android-expo.md Android and Expo adapter
references/sources.md    audited sources and derived principles
ARCHITECTURE.md          scope, authority, and extension model
tests/fixtures/          a provider-neutral dry-run brief
```

## Current status

This MVP defines and validates the agent workflow. It does not bundle a generator, require cloud credentials, or hide platform-tool availability. Platform commands and formats are checked at run time because Apple, Android, and Expo tooling evolve.

The identity turns “icon” into a small visual joke: a single eye-con emerges from the visible remains of several iterations. The full lockup belongs in documentation; the skill avatar keeps only the eye and iteration contours.

## Try the fixture

For a low-risk dry run, use `tests/fixtures/pocket-tide.md` and ask the skill to complete Explore only.
