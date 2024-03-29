# These are a mix of developer test binaries and released binaries.  Some may be broken or bad.  These are not for public mass-consumption. If you do not know any history on them you are at extra risk.  These are being hoarded only because there is no definitive source for storage of these.

# IMUF Binaries
Early binaries may require 4k/4k loops.

# Flasher Tools
* When using Marinus' `IMUF Updater.exe`, must un-check "Original HELIO Firmware" for EmuFlight IMUF Releases.  When using ANY HelioRC release, must check-mark it.  Emu's .BIN are unencrypted, whereas HelioRC's were encrypted.  If flashed with an innappropriate check-mark setting, then reboot FC and wait 5 full minutes for it to reconnect DFU for re-flashing.
* EmuFlight now has a Flasher Tool for OSX, Linux, and Windows.  This tool does not need to select the vendor for encrypted/non-encrypted. https://github.com/emuflight/Nemesis/releases/tag/imuf-flasher-0.1.0

## Marinus Binaries
- F3-V2.01-RC1a.bin
- F3-V2.0.3-RC3.bin
- F3-V2.0.5-RC5.bin
- F3_RC6.bin 			40 fcut frequency
- F3_RC6-B.bin 		80 fcut freq
- F3_RC6_C.bin 		60 fcut
- F3_RC8_acc.bin		First Release Candidate

## Andrey Binary
- *_F3_RC9b.bin			❤️ First Recommended. w/ Configurable LPF (BuF 3.6.6+). Very clean filtering. Shows `208` in diff_*
- IMUF_209.bin    Same, more recently recompiled to show `209` in version/CLI.

## QuickFlash Binaries
- F3_QF.bin 			(210)
- *_F3_211.bin		❤️ Liked_*
- F3_212.bin
- *_RC213.bin 			Released with 0.2.0-RC1_*
- IMUF_215.bin
- IMUF_214.bin
- IMUF_216.bin		Bugged
- IMUF_217.bin		Dynamic.v1
- IMUF_218.bin		Dynamic.far less agressive
- IMUF_219.bin		Dynamic.closer to 216 hopefully it fixes 217-218
- IMUF_220.bin    Just for FillThrillz - closer to 209b
- IMUF_221.bin    Just for FillThrillz - modding the smoothness/sharpness ratio
- IMUF_222.bin    Just for FillThrillz - modding  the smoothness/sharpness ratio
- IMUF_223.bin		Just for FillThrillz - modding  the smoothness/sharpness ratio
- *_IMUF_224.bin		Potential Release_*  - Requires EmuFlight dev version 0.2.31 or *older* **Feels Stiff**.

## Now with `sharpness` - requires 0.2.32 or newer
- IMUF_225.bin 		Sharpness parameter. default 35~=IMUF224; higher=sharper, lower=smoother, 1~=rc209b, 250+=crazy
- IMUF_226.bin    Sharpness default = 75 due refactored multiplier: [226](https://github.com/emuflight/imu-f/commit/9780c1137b74abe29defda9b854cfbf4dbafbc2e) & [0.2.34](https://github.com/emuflight/EmuFlight/commit/dbfca3c25c022d1e71c234cc88a2b37393bca2f5)
- IMUF_227.bin    ❤️ Sharpness default = 1000. More flight efficiency like 221, but better stick feel like 209b: [227](https://github.com/emuflight/imu-f/commit/b330fff9d4119b1255e98e1d477e033b3ccf137c), [227](https://github.com/emuflight/imu-f/commit/8547dd9df2daa450c53c2d26eec45b4139acc8c8) 
- IMUF_228.bin		BUGGED. reported fly-off.  Ramuh test (from RS2K). Sharpness also effects the kalman q like it does for regular fc. Added the kalman Ramuh and made the kalman prediction actually work based on the true acceleration. Requires EmuFlight 0.2.32 or newer.
- IMUF_229.bin      Purge bugged Ramuh, kept the Kalman Prediction.  Good, but requires re-tuning.  Easy to oscillate.
- IMUF_230.bin      **Removed cross-axis influence from covariance.** Built off of 225 (due it flew best for QF) and 226. If you want 230 to fly similar to 226 set your imuf LPF filters to 50 hz. If you want 230 to fly similar to 227 set the IMUF lpf filters to 10hz.
- IMUF_231.bin     Back-ported Paweł Spychalski's covarience math.

## All 230.X, 231.X, 240, 240.X are highly recommended to **not** use; Some of these require a special build of helio/strix .hex for setting test-values.

## Latest
- `9001`❤️ is good and flyable, but removes sharpness. `9002`❤️ re-adds sharpness.  Both have static LPF.
- IMUF_250.bin    ❤️ Released verion of 9002. Sharpness can be turned off with `sharpness=0`.
- IMUF_251.bin    testing binary. may rocket. move kalman prediction after biquad filter.
- IMUF_252.bin    ❤️ testing binary. removed sharpness in totality. equivalent to 9001, but latest code base.
- IMUF_253.bin    testing binary.  incomplete. fixed butoffs, improved kalman, but not yet "more static" k, nor pt2.
- IMUF_254_PT2.bin ❤️
- IMUF_255_PT3.bin ❤️
- IMUF_256_PTN.bin ❤️ Pilot selectable PT(n) via `set ptn_order = `


## Old HelioRC recompiled
- IMUF_107_flash-with-unchecked-orig-helio.bin
- Original HelioRC: https://github.com/heliorc/imuf-release-dev
