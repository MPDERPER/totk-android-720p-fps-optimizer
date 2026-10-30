# Provenance and inspection

Upstream repository: https://github.com/MaxLastBreath/nx-optimizer
Pinned revision: bd98bb3c9ee7eb16c2dd3c51a8c6ecf168330cf3

Both supplied binary files are byte-for-byte identical to the following upstream files at the pinned revision:

| File | Upstream Git blob SHA-1 | SHA-256 |
| --- | --- | --- |
| main.npdm | 27a5cd21a43fac1e0aa48fbb940ff555f14a3f78 | d593a80e5e53f8603afab0655af31bac0aa37ebf8ab8e205017e38b581d9a006 |
| subsdk3 | cecbbb19b3e86e7bcf03fb68241979bdbde62c14 | 930e4e995239bb40a4f68fb1a237bcf1b28aa9ce0a581533f8a02a92f76472a6 |

Source directory: https://github.com/MaxLastBreath/nx-optimizer/tree/bd98bb3c9ee7eb16c2dd3c51a8c6ecf168330cf3/src/PatchInfo/Tears%20Of%20The%20Kingdom%20OLD/UltraCam/exefs
License notice: https://github.com/MaxLastBreath/nx-optimizer/blob/bd98bb3c9ee7eb16c2dd3c51a8c6ecf168330cf3/LICENSE.md

The pinned upstream tree contains one license file, LICENSE.md, declaring CC BY-NC 2.0. Its notice is included verbatim as LICENSE.upstream.md. The author describes UltraCam as distributing original code rather than game assets: https://www.patreon.com/MaxLastBreath/about

The updated RAR contains exactly three files: the two binary files above and `romfs/UltraCam/maxlastbreath.ini`. The updated INI has SHA-256 `b5ec29c8549415c12c81e818c4f1e0675e660746f00e8c47282377ec8cdd21c1`. No supplied README, installation guide, credits, or license file existed; these have been added.

The configuration is preserved exactly. The source archive name mentions 60fps, but its actual gameplay cap is 59. The release name reflects the actual settings.

main.npdm is executable metadata and subsdk3 has an NSO0 executable header. They were inspected and compared, not executed. No game ROM, update, firmware, keys, textures, models, music, or screenshots were found among the supplied files. No independent ownership audit of upstream code was performed.

Validation is static only. No Android device, Eden installation, game session, or performance benchmark was run.
