# Apple adapter

Use current Apple documentation and installed tool help as the authority for the detected Xcode/Icon Composer version.

## Route

1. Determine the target OS versions, Xcode version, and whether Icon Composer plus its command-line tooling are installed.
2. Decide whether the artwork benefits from an Icon Composer `.icon` package. Use layers only for meaningful depth/material/appearance behavior; retain a conventional source fallback when the deployment target or build chain needs it. Do not hand-author undocumented `.icon` internals as a stable contract.
3. Prepare supported SVG or PNG layers with clean bounds and intentional transparency. Keep visual effects editable when the tool is expected to render them.
4. Build or validate the package with available Apple tooling. Discover `ictool` and its help at runtime where supported; its path and CLI are version-sensitive. Prefer automation over asking the user to open Icon Composer manually.
5. Configure the detected Apple project or Expo version using its current supported path. Validate with the actual build tools when possible.

## Appearances and checks

Preview every appearance required by the detected tool and target—currently including default, dark, clear, and tinted variants on relevant Apple platforms—using platform behavior rather than recoloring by assumption. Confirm the focal symbol, contrast, and material survive system treatment and small rendering.

For a PNG fallback, use the dimensions required by the project—commonly a 1024×1024 iOS source—and verify it is square, full-bleed, unmasked, and opaque. Treat watchOS and other platform layouts separately rather than resizing an iOS assumption.

If Icon Composer or automation is unavailable, deliver named layer sources, a composition note, expected appearances, and exact import/export/validation steps. State which steps remain unverified.
