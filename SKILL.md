---
name: one-good-icon
description: Explore, critique, refine, and package app icons from real product or brand material. Use for app-icon direction, small-size and platform validation, Apple Icon Composer assets, Android adaptive/themed icons, or Expo icon configuration.
---

# One Good Icon

Create one recognizable, resilient app icon through three gated phases: **Explore → Refine → Ship**. Keep the selected origin, evidence, and human decisions traceable.

## Establish the run

Inspect the actual product material before proposing imagery: product and brand docs, UI, assets, screenshots, references, sketches, an existing icon, or a selected generated concept. Record:

- product promise, audience, personality, and recognition target;
- platform and stack constraints;
- visual principles worth preserving: composition, geometry, contrast, material, depth, color, density, and character;
- proprietary forms to avoid reproducing.

Treat references as evidence, not a style order. Extract transferable principles and create an original symbol. When MAYA is active, it owns the wider art direction and global critique; One Good Icon owns app-icon exploration, validation, and delivery.

Identify the current phase from the user's confirmed decisions. Selection advances Explore to Refine. Explicit approval of one icon advances Refine to Ship. A request to package an already approved icon may start at Ship after confirming the source master and approval.

## Explore

Read [references/explore.md](references/explore.md). Produce about 4–6 materially different, named directions. Use the host's native image-generation capability when available. Otherwise provide generator-ready prompts and a comparison plan.

Present the directions together in a clear board with their thesis and tradeoff. Stop for a human choice. Exploration is complete when the user selects one or two candidates; do not begin reconstruction, platform packaging, or the full test matrix before that choice.

## Refine

Read [references/refine.md](references/refine.md) and [references/critic.md](references/critic.md). Generate targeted variations of only the selected candidates, then run the tests that expose actual failure modes:

- size: 1024, 256, 128, 64, and 32 px;
- environment: light, dark, and visually busy surroundings;
- competition: realistic home-screen or category grids;
- platform: relevant iOS appearances and Android masks/themed-icon behavior.

Report concrete observations, not scores. A useful finding names the feature, condition, and consequence: “the inner counter closes at 32 px, so the mark becomes a blob.” Taste or Impeccable may provide a second aesthetic opinion when available; the icon critic remains primary.

Stop for explicit approval of one candidate. Refine is complete only when the chosen origin is identified and the user approves it for production.

## Ship

Read [references/ship.md](references/ship.md), then load only the platform adapter needed:

- Apple or Icon Composer: [references/apple.md](references/apple.md)
- Android, Expo, or mixed mobile stacks: [references/android-expo.md](references/android-expo.md)

Choose the production representation from the artwork:

- simple geometric construction: reconstruct as vector when it improves editability and precision;
- complex illustration, texture, or painterly light: retain a high-quality raster master;
- Icon Composer: separate only layers with a real material, depth, or appearance role.

Preserve the selected origin alongside derived assets. Use available platform tools to build and verify outputs; automate Icon Composer work when the environment supports it and give a precise fallback when it does not. Adapt to the detected stack instead of claiming unsupported packaging.

Finish when required files exist, configuration points to them, platform validators pass where available, and rendered context checks reveal no blocking defects. Report delivered files, verification evidence, fallbacks, and deferred platform work.

## Tool and companion policy

- Image generation is capability-based and provider-agnostic. Prefer the host's native ImageGen; require no API key or third-party generator.
- If generation is unavailable, deliver complete prompts with aspect, composition, exclusions, and reference principles.
- One Good Icon is the complete app-icon workflow. It does not require or discover external icon-generation skills, API-backed CLIs, or provider credentials.
- MAYA, Taste, Impeccable, or prototype may contribute art direction or a second opinion when already available; none is required for completion.
- Use prototype's divergence principle—distinct hypotheses with named axes—without building HTML/CSS/SVG stand-ins for visual icon exploration.
- Keep future platform support behind new adapter references; preserve the three-phase contract.
