# Explore dry run

The fixture `fixtures/pocket-tide.md` was exercised with no ImageGen capability.

Result: five distinct named directions, each with a product rationale, preserved reference principles, a specific tradeoff, and a provider-neutral 1024×1024 prompt. The response used a text comparison board, requested selection of one or two directions, and stopped without SVG reconstruction, layers, platform packaging, or Refine tests.

Observed ambiguity: “board” was not explicit in the no-ImageGen branch. `references/explore.md` now specifies a compact comparison table plus complete per-direction prompts for that fallback.

