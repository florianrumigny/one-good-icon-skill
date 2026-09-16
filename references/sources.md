# Audited sources

Checked 2026-09-16. Use these links to refresh version-sensitive facts; the operational rules live in the phase and platform references.

## Prior art

- [xzhih/app-icon-skill at audited commit](https://github.com/xzhih/app-icon-skill/tree/08e5b084f3e179b6d12546614902b293c5ee0b91): audited for source routing, origin preservation, evidence-led reconstruction, semantic layers, and verification. This is research provenance only, not a runtime integration or dependency.
- [Code with Beto app-icon skill at audited commit](https://github.com/Code-with-Beto/skills/blob/f35f3d9ce5da881527b9eaf03ca37e73382e9149/plugins/cwb-app-icon/skills/app-icon/SKILL.md) and [SnapAI at audited commit](https://github.com/Code-with-Beto/snapai/tree/a60d5393287cbf46794507e6ee0ff54d689d5976): audited for prompt enhancement and Expo packaging ideas. They are research sources only; One Good Icon replaces their runtime role and requires neither installation, provider keys, nor model-specific behavior.

Corrections carried into this skill:

- transparency is an output/layer decision, not a universal icon requirement;
- Android foreground, background, and monochrome are deliberate roles, not one reused PNG;
- a flattened image in a hand-written `.icon` bundle is not proof of a valid layered Icon Composer delivery;
- the Android 66×66 safe region belongs to a 108×108 adaptive-icon canvas and is not a universal resize percentage.

## Platform authorities

- [Apple HIG: App icons](https://developer.apple.com/design/human-interface-guidelines/app-icons), [Icon Composer](https://developer.apple.com/icon-composer/), [Xcode integration](https://developer.apple.com/documentation/Xcode/creating-your-app-icon-using-icon-composer), [WWDC25 visual guidance](https://developer.apple.com/videos/play/wwdc2025/220/), and [WWDC25 Icon Composer session](https://developer.apple.com/videos/play/wwdc2025/361/). These support one core idea, unmasked source art, restrained useful layers, platform appearances, and tool-based verification. Apple does not publish a stable `ictool` CLI or `.icon` JSON contract; discover local capabilities at runtime.
- [Android adaptive icon guidance](https://developer.android.com/develop/ui/compose/system/icon_design_adaptive): separate foreground/background layers, 108×108 dp canvas, central 66×66 dp guaranteed safe region, multiple masks, and a purpose-made monochrome layer for predictable themed icons.
- [Expo icon guide](https://docs.expo.dev/develop/user-interface/splash-screen-and-app-icon/) and [Expo app config](https://docs.expo.dev/versions/latest/config/app/): common and platform overrides, adaptive and monochrome keys, `.icon` support from SDK 54, opaque full-bleed iOS PNG fallback, and the distinction between Prebuild/CNG and manually owned native projects.

## Professional design evidence

- [Microsoft app icon guidance](https://learn.microsoft.com/en-us/windows/apps/design/iconography/app-icon-design): singular metaphor, balanced silhouette, limited detail, and purposeful perspective.
- [IBM app icon guidance](https://www.ibm.com/design/language/iconography/app-icons/usage/): optical alignment, explicit small-size inspection, consistent weight, and gallery/context comparison.
- [Michael Flarup interview](https://blog.adobe.com/en/publish/2015/07/23/flarup-app-icon) and [Let's Talk Icons](https://old.applypixels.com/lets-talk-icons/): an app icon is a product-specific visual anchor optimized for its square canvas, sizes, and contexts—not merely a logo export.

## Local companion principles

- MAYA: real material first, explicit divergent hypotheses, evidence-backed critique, and human selection; it retains overall art-direction authority when present.
- prototype: every candidate needs a named axis and an honest tradeoff; near-duplicates do not count as divergence.
- Impeccable: the brief wins, incumbent identity is preserved during refinement, and QA is bounded.
- Taste: retain intentionality and anti-default critique only; webpage-specific rules are irrelevant to app icons.
