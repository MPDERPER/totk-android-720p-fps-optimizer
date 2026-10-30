# TOTK Android 720p FPS Optimizer

An Android-focused UltraCam FPS optimizer configured by **MPDERPER** for *The Legend of Zelda: Tears of the Kingdom*. It targets **1280 × 720** with a **59 FPS cap** and graphics settings intended to reduce rendering cost. The underlying UltraCam implementation is by **MaxLastBreath**.

**Reported performance:** MPDERPER reports **30+ FPS with frame generation on Eden Nightly**. This is a user report, not an independently verified benchmark. No device specifications, Eden build number, game version, driver version, test scene, frame-time capture, or frame-generation method were supplied. It is unknown whether the reported counter includes generated frames. A 59 FPS cap is a configuration target, not a promise of sustained 59 FPS or 60 FPS gameplay. This package does not provide or enable frame generation itself.

## Settings included

The original `maxlastbreath.ini` is preserved byte-for-byte.

| Setting | Value | Meaning / limitation |
| --- | --- | --- |
| Resolution | `Width = 1280`, `Height = 720` | Configured 720p rendering target; actual behavior depends on the bundled UltraCam build and emulator settings. |
| Gameplay cap | `MaxFramerate = 59` | Requested maximum frame rate. |
| Menu cap | `MenuFPSLock = 59` | Requested menu frame-rate limit. |
| Movies | `MovieFPS = 29` | Separate movie frame-rate setting. |
| Emulator scale | `EmuScale = 1.0` | Preset scale value; emulator-side scaling must also be checked. |
| Shadows | `ShadowResolution = 206` | Reduced shadow-resolution setting; potential visual-quality tradeoff. |
| Render distance | `RenderDistance = 10000` | Configured distance; no measured speedup is claimed. |
| Quality options | `QualityImprovements = On`, `DisableFXAA = On` | Enables the named UltraCam options and requests FXAA removal. |
| Depth of field / lens flare | `RemoveDepthOfField = On`, `RemoveLensflare = On` | Requests removal of both effects to reduce post-processing work and visual clutter. No independent performance gain was measured. |
| Fog | `DisableFog = Off` | This preset does not request fog removal. |
| Field of view | `Fov = 55` | Preset camera field of view. |
| Handheld / portable mode | `Width = 1280`, `Height = 720`, `OverrideHandheld_Resolution = On` | Requests the 1280 × 720 handheld resolution override. Actual output still depends on UltraCam and emulator behavior. |
| Benchmark selector | `Benchmark = 1` | A configuration value only; no benchmark was run for this release. |

The graphics optimizations above are configuration choices, not independently measured improvements.

## Installation on Android / Eden

These are layout-based installation instructions. They have not been tested in a live Eden Nightly session, and menu names vary between builds.

1. Back up your saves and existing mod configuration. Close the game before changing mod files.
2. Download and extract the release ZIP. The folder `TOTK Android 720p FPS Optimizer` must contain both `exefs` and `romfs` directly beneath it.
3. Use Eden's per-game mod/add-on management for Tears of the Kingdom to install or select that mod folder. If your build uses a mod directory instead of an importer, place the complete folder in the game's mod/load directory, preserving the layout below. If an importer accepts ZIPs, confirm it recognizes the nested mod folder; otherwise use the extracted folder.
4. Enable this mod. Disable other mods that replace `exefs/main.npdm`, `exefs/subsdk3`, or the same UltraCam configuration, and avoid stacking conflicting FPS/resolution mods.
5. Check emulator resolution scaling separately. The supplied preset uses `EmuScale = 1.0` and enables the 1280 × 720 handheld/portable override.
6. Start the game and check stability, game speed, image quality, and frame pacing. If the mod causes problems, disable it and restore your backup.

```text
TOTK Android 720p FPS Optimizer/
├── exefs/
│   ├── main.npdm
│   └── subsdk3
└── romfs/
    └── UltraCam/
        └── maxlastbreath.ini
```

The bundled files match the upstream **Tears Of The Kingdom OLD** UltraCam payload. Exact game-update compatibility and Android/Eden compatibility have not been independently established. Do not assume the compatibility list for the current upstream UltraCam release applies to this older binary. Obtain game/update compatibility guidance from [MaxLastBreath's upstream project](https://github.com/MaxLastBreath/nx-optimizer).

Frame generation, where available in your setup, is configured separately. Generated display frames should be reported separately from native game FPS. This release includes no emulator, GPU driver, frame-generation software, game, update, firmware, keys, or game media assets.

## Credits and redistribution

- **MPDERPER:** supplied Android preset, packaging, and the reported Eden Nightly performance claim.
- **MaxLastBreath:** UltraCam and NX Optimizer, including the unchanged upstream binary payload. See [CREDITS.md](CREDITS.md).

The bundled upstream material is distributed under **Creative Commons Attribution-NonCommercial 2.0 Generic (CC BY-NC 2.0)**. Preserve attribution and license notices, and do not use that material commercially. See [LICENSING.md](LICENSING.md), [the original license notice](LICENSE.upstream.md), and the [binary provenance record](PROVENANCE.md). No endorsement by MaxLastBreath, Nintendo, or Eden is claimed.

## Validation

Static checks verified archive contents, exact copies of the provided files, binary matches to the pinned upstream source, and release ZIP integrity. **No game launch, Android device test, frame-generation test, or independent performance benchmark was performed.**

