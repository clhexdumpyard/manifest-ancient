-----------------------------------------------------------------------------

<p align="center">
 <img src="https://github.com/Ancient-Roms/manifest/blob/eleven/ancient.png" > 
</p>

-----------------------------------------------------------------------------
Credits:
=======
 * [**AOSP**](https://android.googlesource.com)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**SuperiorOS**](https://github.com/SuperiorOS)
 * [**DotOS**](https://github.com/DotOS)
 * [**PixelExperience**](https://github.com/PixelExperience)
 * [**AospExtended**](https://github.com/AospExtended)
 * [**Syberia OS**](https://github.com/syberia-project)
 * [**Nitrogen OS**](https://github.com/nitrogen-project)
 * [**Pixys OS**](https://github.com/PixysOS)
 * [**ArrowOS**](https://github.com/ArrowOS)
 * [**MSM-Xtended**](https://github.com/Project-Xtended)
 * [**HavocOS**](https://github.com/Havoc-OS)
 * [**BootleggersROM**](https://github.com/BootleggersROM)
 * [**ABC**](https://github.com/ezio84?tab=repositories)
 * [**DerpFest**](https://github.com/derplab)
 * [**Evolution-X**](https://github.com/evolution-x)
 * [**OMNIROM**](https://github.com/omnirom)
 * [**AOSIP**](https://github.com/aosip)
 * [**Resurrection Remix**](https://github.com/ResurrectionRemix)
 * [**Dirty Unicorns**](https://github.com/DirtyUnicorns)
 * [**Bliss**](https://github.com/blissroms)
 * [**ExtendedUI**](https://github.com/extended-ui)
 * [**AICP**](https://github.com/aicp)
 * [**MoKee**](https://github.com/Mokee)
 * [**RevengeOS**](https://github.com/revengeos)
 * [**POSP**](https://github.com/PotatoProject)
 * [**ION**](https://github.com/i-o-n)
 * [**crDroid**](https://github.com/crdroidandroid)
 * [**GZOSP**](https://github.com/GZOSP)
 * [**Colt-Enigma**](https://github.com/Colt-Enigma)
 * [**YAAP**](https://github.com/yaap)

-----------------------------------------------------------------------------

To get started with the building process, you'll need to get familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

# To initialize your local repository for Ancient, use a command like this:-

```bash
 $ repo init -u https://github.com/Ancient-Lab/manifest -b eleven
```

# Then to sync up:- 

```bash
 $ repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

# Follow our ancient_device.mk:-
```bash
 $(call inherit-product, vendor/ancient/config/common_full_phone.mk)
```

# Start the build:-

```bash
 $ . build/envsetup.sh
 $ lunch ancient_<devicecodename>-userdebug
 $ mka bacon -j$(nproc --all)
```
-----------------------------------------------------------------------------
