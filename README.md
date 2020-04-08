# IMUF Binaries
Early binaries may require 4k/4k loops.

When using Marinus' `IMUF Updater.exe`, must un-check "Original HELIO Firmware" for these.  When using ANY Helio release, must check-mark it.  These .BIN are unencrypted, whereas HELIO's were encrypted.  If flashed with innappropriate check-mark, then reboot FC and wait 5 full minutes for it to reconenct for re-flashing.

## Marinus Binaries
- F3-V2.01-RC1a.bin
- F3-V2.0.3-RC3.bin
- F3-V2.0.5-RC5.bin
- F3_RC6.bin 			40 fcut frequency
- F3_RC6-B.bin 		80 fcut freq
- F3_RC6_C.bin 		60 fcut
- F3_RC8_acc.bin		First Release Candidate
- *_F3_RC9b.bin			First Recommended. w/ Configurable LPF (BuF 3.6.6+). Very clean filtering. Shows `208` in diff_*

## QuickFlash Binaries
- F3_QF.bin 			(210)
- *_F3_211.bin			Liked_*
- F3_212.bin
- *_RC213.bin 			Released with 0.2.0-RC1_*
- IMUF_215.bin
- IMUF_214.bin
- IMUF_216.bin		Bugged
- IMUF_217.bin		Dynamic.v1
- IMUF_218.bin		Dynamic.far less agressive
- IMUF_219.bin		Dynamic.closer to 216 hopefully it fixes 217-218
- IMUF_221.bin
- IMUF_222.bin
- IMUF_223.bin		Just for FillThrillz
- *_IMUF_224.bin		Potential Release_*  - Requires EmuFlight dev version 0.2.31 or *older*

## Now with `sharpness` - requires 0.2.32 or newer
- IMUF_225.bin 		Sharpness parameter. default 35~=IMUF224; higher=sharper, lower=smoother, 1~=rc209b, 250+=crazy
- IMUF_226.bin    Sharpness default = 75 due refactored multiplier: [226](https://github.com/emuflight/imu-f/commit/9780c1137b74abe29defda9b854cfbf4dbafbc2e) & [0.2.34](https://github.com/emuflight/EmuFlight/commit/dbfca3c25c022d1e71c234cc88a2b37393bca2f5)
- IMUF_227.bin    Sharpness default = 1000. More flight efficiency like 221, but better stick feel like 209b: [227](https://github.com/emuflight/imu-f/commit/b330fff9d4119b1255e98e1d477e033b3ccf137c), [227](https://github.com/emuflight/imu-f/commit/8547dd9df2daa450c53c2d26eec45b4139acc8c8) 
- IMUF_228.bin		Ramuh test (from RS2K). Sharpness also effects the kalman q like it does for regular fc. Added the kalman Ramuh and made the kalman prediction actually work based on the true acceleration. Requires EmuFlight 0.2.32 or newer.
- IMUF_229.bin Purge bugged Ramuh, kept the Kalman Prediction.
