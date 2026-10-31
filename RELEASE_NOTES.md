# v1.3.1 — stable 30 FPS configuration update

Updated Android FPS optimizer from MPDERPER with MaxLastBreath's unchanged legacy UltraCam payload.

- Configured resolution: **1280 × 720**.
- Gameplay and menu cap: **59 FPS**; movie setting: **29 FPS**.
- Disables ambient occlusion, screen-space reflections, volumetric fog, and bloom.
- Reduces `RenderDistance` from `10000` to `5000`.
- Reduces `Fov` from `55` to `45`.
- Retains `ShadowResolution = 206`, `QualityImprovements = On`, and `DisableFXAA = On`.
- Removes depth of field with `RemoveDepthOfField = On`.
- Removes lens flare with `RemoveLensflare = On`.
- Enables the **1280 × 720 handheld/portable resolution override** with `OverrideHandheld_Resolution = On`.
- **Reported performance:** MPDERPER reports **stable 30 FPS without frame generation** using this v1.3.1 configuration. This has not been independently verified. Hardware, emulator build, driver, game version, test scene, frame-time capture, and test duration were not supplied. The 59 FPS cap remains a configuration target rather than a performance guarantee.

Extract the attached Android mod ZIP and install the `TOTK Android 720p FPS Optimizer` folder through your emulator's per-game mod management, preserving `exefs` and `romfs`. See the repository README for detailed instructions, conflicts, and compatibility limitations. Installation has not been tested in a live Eden session.

**Credits:** UltraCam / NX Optimizer by [MaxLastBreath](https://github.com/MaxLastBreath/nx-optimizer); Android configuration and performance report supplied by MPDERPER. Upstream binaries are redistributed unchanged under [CC BY-NC 2.0](https://creativecommons.org/licenses/by-nc/2.0/), with source hashes and notices included. No game ROM, update, keys, firmware, emulator, or game media assets are included.

Validation covers static file inspection, upstream binary identity, and ZIP integrity. No independent gameplay or performance benchmarks were performed. Exact game-update compatibility of the legacy payload is unverified.

