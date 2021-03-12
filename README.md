```bash


```
You can alternatively use this command to save some space and time :

```bash
repo init --depth=1 -u https://github.com/Deluxe-AOSP/manifest.git -b 11

```

Then to sync up:

```
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
You can just use `repo sync` or above command, but this will save you from lot of terminal spam, data and time.
```bash
repo sync -c -q --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune -j$(nproc --all)
```
---------------------------------------------------------------------------------------
 Compilation of  LegionOS:
 ==================

From root directory of project, perform following commands in terminal

```bash
$ . build/envsetup.sh
$ lunch legion_<device_codename>-buildtype
$ make legion
```
---------------------------------------------------------------------------------------
 Credits:
 =======

 * [**LineageOS**](https://github.com/LineageOS)
 * [**Xtended**](https://github.com/Project-Xtended)
 * [**Colt**](https://github.com/Colt-Enigma)
 * [**ROS**](https://github.com/RevengeOS)
 * [**ManyMore from where cherry-picked from**](https://github.com)

---------------------------------------------------------------------------------------
