# Refine

Use this phase only for one or two candidates selected by the user.

## Target variations

Carry forward the candidate's recognition anchor. Generate a small, purposeful set where each variation tests a named uncertainty: silhouette width, negative-space aperture, depth, perspective, palette, material, or background relationship. Avoid reopening unrelated directions.

Keep the selected Explore origin immutable. Link every variation to its parent and retain prompts or generation metadata.

## Test in evidence-producing order

1. **Size:** inspect 1024, 256, 128, 64, and 32 px at actual display size. Check which internal gaps, edges, highlights, and semantic cues survive.
2. **Environment:** place the icon on light, dark, and visually busy backgrounds. Check boundary loss, glow/halo artifacts, and dependence on a single wallpaper value.
3. **Competition:** compare in a realistic home-screen or category grid at equal size. Look for category cliché, confusing neighbors, weak visual weight, or artificial loudness.
4. **Platform:** preview relevant Apple appearances and Android masks. Test monochrome/themed behavior only when it is part of the requested delivery.

Use realistic masks and platform renderers when available. Never alter the master merely to make a flawed preview tool look good.

## Decide with observations

Run the specialist review in `critic.md`. Summarize:

- what remains recognizable across tests;
- the highest-impact failure and where it occurs;
- the smallest edit likely to fix it;
- tradeoffs that require human judgment.

Do not calculate a total or weighted score. Apply a bounded repair pass, rerun affected tests, and present the evidence. Complete Refine only after the user explicitly approves one icon for Ship.

