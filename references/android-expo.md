# Android and Expo adapters

Use current Android and Expo documentation plus detected project versions as the authority.

## Android

For an adaptive icon, prepare a foreground and a deliberate background color or image. On the current Android model, each layer occupies a 108×108 dp canvas and the central 66×66 dp is guaranteed safe across masks; use those as platform geometry, not as a universal 66% resize recipe. Preview multiple launcher masks and do not pre-mask the source into a rounded square or circle.

Add a monochrome layer when themed icons are requested or supported by the target. Design it as a true single-color recognition shape, not an automatic grayscale conversion. Retain legacy/fallback icons when required by the project's minimum SDK or build setup.

Validate resource names, XML/config references, dimensions, transparency, safe-zone behavior, and rendered results on available emulator/device tooling.

## Expo

Detect the Expo SDK and whether configuration lives in `app.json`, `app.config.js`, or `app.config.ts`. Inspect existing config before editing.

- Configure the top-level app icon through the field supported by the detected SDK.
- Configure Android adaptive icon foreground/background and monochrome fields only when supported by that version.
- Use an Apple `.icon` asset only when the detected Expo version and Apple build path document support. Current support begins with Expo SDK 54; otherwise use the supported raster/asset-catalog route.

Resolve paths from the config file, preserve dynamic config behavior, and avoid replacing unrelated settings. Determine whether Expo Prebuild/CNG owns the native projects; editing app config alone does not update a manually maintained native project. Run the project's normal config/build inspection when available, then verify that resolved native projects point to the delivered assets.

For non-Expo React Native or native Android projects, use their actual resource/config conventions instead of applying Expo fields.
