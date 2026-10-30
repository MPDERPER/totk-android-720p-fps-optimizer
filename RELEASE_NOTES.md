# v1.2.0 — shadow optimization update

Updated Android FPS optimizer from MPDERPER with MaxLastBreath's unchanged legacy UltraCam payload.

- Configured resolution: **1280 × 720**.
- Gameplay and menu cap: **59 FPS**; movie setting: **29 FPS**.
- Changes `ShadowResolution` from `205` to `206` while retaining `RenderDistance = 10000`, `QualityImprovements = On`, and `DisableFXAA = On`.
- Removes depth of field with `RemoveDepthOfField = On`.
- Removes lens flare with `RemoveLensflare = On`.
- Enables the **1280 × 720 handheld/portable resolution override** with `OverrideHandheld_Resolution = On`.
- **Reported performance:** MPDERPER reports **30+ FPS with frame generation on Eden Nightly**. This has not been independently verified. Hardware, build versions, test conditions, native FPS, and generated-frame contribution were not supplied. The cap is not a performance guarantee.
- Frame generation is not bundled or enabled by this package.

Extract the attached Android mod ZIP and install the `TOTK Android 720p FPS Optimizer` folder through your emulator's per-game mod management, preserving `exefs` and `romfs`. See the repository README for detailed instructions, conflicts, and compatibility limitations. Installation has not been tested in a live Eden session.

**Credits:** UltraCam / NX Optimizer by [MaxLastBreath](https://github.com/MaxLastBreath/nx-optimizer); Android preset and performance report supplied by MPDERPER. Upstream binaries are redistributed unchanged under [CC BY-NC 2.0](https://creativecommons.org/licenses/by-nc/2.0/), with source hashes and notices included. No game ROM, update, keys, firmware, emulator, or game media assets are included.

Validation covers static file inspection, upstream binary identity, and ZIP integrity. No independent gameplay or performance benchmarks were performed. Exact game-update compatibility of the legacy payload is unverified.

