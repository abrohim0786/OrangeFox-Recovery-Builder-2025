# compile OrangeFox Recovery with Github Actions
```
only Supports OrangeFox  (14.1 is not ready yet) / 12.1 / 11
**************
*** WARNING***: the fox_14.1 branch is *EXPERIMENTAL*! Also, syncing will take a *VERY* long time
**************
```
![cap_sprout](https://wiki.orangefox.tech/banner.svg)
---
# Features
Auto updates in background/
Installing old releases/
Ability to create and edit OpenRecoveryScripts/
Beautiful UI/
No analytics/ads, small apk size/
Internal Storage (Yes, decryption works!)/
External Storage (Both OTG and MicroSD.)/
Touchpanel/
Brightness/
Vibration/Haptic/
ADB Sideload/
MTP/
Flashlight/
Synced with the latest Teamwin changes/
Designed with latest Material design 2 guidelines/
Implemented support for Flyme and MIUI OTA, and incremental block-based OTA in custom ROMs/
Included assorted customizations/
Inbuilt patches, like Magisk and password reset patch/
Several addons/
Password protection/
Fully open-source/
Frequently updated/
# Why OrangeFox Recovery?
We have been operating since early 2018. Since then we have improved the quality, stability, and device support of the recovery. Today OrangeFox is the leader in stability, UI design, and UX. Installing OrangeFox means being with the latest code and fastest fixes.

OrangeFox Recovery was originally designed for Xiaomi Redmi Note 4X Snapdragon (mido). Right now we support 50+ devices, with more than 5 million downloads from our official download server.


## Release Notes
```
= 2025-07-19
- fix problem with device tree link in release!

= 2024-10-21
- Fix issue with Snapdragon Gen 7/8 devices

= 2024-10-06
- fix some errors
- fix problems with vendor_boot
- Include Recovery to tar for Samsung devices
- Include recovery installer zip
- LDCheck for checking missing dependencies.
- Clarify options in README
- Increase swap size for kernel inline builds
- Remove common tree input fields (not needed)
- Fix build with Omni manifests
- Update ubuntu to latest version 
- Updated to work with Android 14 AOSP minimal TWRP manifest
- Completely reconstruct the use logic to reduce the difficulty of use
- Optimize the parameter transfer part, now you can run multiple Workers at the same time
```

-----

## Output will be like this
![](https://s3.bmp.ovh/imgs/2024/10/07/3913c62d5c20649f.png)

## Parameter Description
| Name | Description | Example |
| ------------ | -------------------- | ------------ |
| `MANIFEST_BRANCH` | Source branch | OrangeFox-12.1 |
| `DEVICE_TREE_URL` | Device tree address | https://github.com/kinguser981/android_device_samsung_a05s.git |
| `DEVICE_TREE_BRANCH` | Device branch that you want to use for build (typically corresponds to the manifest branch) | android-12.1 |
| `DEVICE_PATH` | Device tree location for syncing, relative to workspace root (usually listed as "LOCAL_PATH" or "DEVICE_PATH" in BoardConfig.mk) | device/samsung/a05s |
| `DEVICE_NAME` | Model name (same as twrp_`<DEVICE_NAME>`.mk from device tree) | a05s |
| `DEVICE_MAKEFILE` | Name of device-specific makefile from tree (format: `<PREFIX>_<DEVICE_NAME>`) | fox_a05s.mk
| `BUILD_TARGET` | Build Target Partition (boot/recovery/vendor_boot) | recovery |
| `RECOVERY_INSTALLER` | Include recovery installer zip | Optional |
| `RECOVERY_TAR` | Recovery to tar for Samsung devices | Optional |

-----

## Usage Instructions

#### 1. Click 'Fork' in the upper right corner of this repo
![](https://s3.bmp.ovh/imgs/2024/09/07/acd37b59bde6971e.png)
#### 2. After waiting for the automatic redirection, you will see your own username
## Building the Recovery
#### 3. Click on 'Actions' then Click no 'OrangeFox - Build'
![](https://s3.bmp.ovh/imgs/2024/10/07/fc95db719a8603e4.png)
#### 4. Click 'Run workflow', choose the branch for the recovery that you want to build, and fill in according to the above 'Parameter Description'
![](https://s3.bmp.ovh/imgs/2024/10/08/b0914297dd7ec359.png)
#### 5. After filling in, click 'Run workflow' to start running

-----

## Compilation results
Can be downloaded at [Release](../../releases)

-----
## Reference and Credits
- https://github.com/that1
- https://github.com/TeamWin
- https://gitlab.com/OrangeFox
- https://github.com/cd-Crypton
- https://github.com/azwhikaru
- And to all Contributors in every repositories and scripts I used.

