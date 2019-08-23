[![Build status](https://ci.appveyor.com/api/projects/status/wwokiviriq3m52t6?svg=true)](https://ci.appveyor.com/project/ThirteenAG/gtaiv-eflc-fusionfix)
[![Build Status](https://dev.azure.com/thirteenag/GTAIV.EFLC.FusionFix/_apis/build/status/ThirteenAG.GTAIV.EFLC.FusionFix?branchName=master)](https://dev.azure.com/thirteenag/GTAIV.EFLC.FusionFix/_build/latest?definitionId=1&branchName=master)
[![Discord](https://img.shields.io/badge/chat-on%20discord-7289da.svg?logo=discord)](https://discord.gg/y2cZFRA)

<p align="center">
  <img height="100" src="https://user-images.githubusercontent.com/4904157/63623173-921aaf00-c601-11e9-8b84-fc5803269323.png">
</p>

# GTAIV.EFLC.FusionFix

This projects aims to fix some issues in Grand Theft Auto IV and Episodes from Liberty City.

Changelog:

- [Fixed recoil behavior that was different when playing with keyboard/mouse and gamepad](https://github.com/GTAmodding/GTAIV-Issues-List/issues/6)
- [Fixed forced "definition off" setting in cutscenes, now cutscenes will respect the menu setting](https://github.com/GTAmodding/GTAIV-Issues-List/issues/5)
- [Partially fixed emissive shader bug, namely BAWSAQ building is still rendered incorrectly, but the rest of the lights are now present in the game (e.g. Rotterdam Tower, Comrades Bar area)](https://github.com/GTAmodding/GTAIV-Issues-List/issues/4)
- [Fixed DLC car lights in TBoGT](https://github.com/GTAmodding/GTAIV-Issues-List/issues/3)
- [Tree foliage casts dynamic shadows instead of static](https://github.com/GTAmodding/GTAIV-Issues-List/issues/9)

## Installation:

#### GTAIV 1.0.8.0 / GTAIV 1.0.8.0 + DLC Episodes / GTA EFLC 1.0.3.0

This fix is tested only with latest official update and [XLiveLessAddon](https://bitbucket.org/ThirteenAG/xlivelessaddon/downloads/).

The following installation instructions assume that you're either have it already, or willing to install it.
Online features of the game are not available with [XLiveLessAddon](https://bitbucket.org/ThirteenAG/xlivelessaddon/downloads/).

---

If you only want the core package, that includes all aforementioned fixes,

### **Download**: [GTAIV.EFLC.FusionFix.Min.zip](https://github.com/ThirteenAG/GTAIV.EFLC.FusionFix/releases/latest/download/GTAIV.EFLC.FusionFix.Min.zip)

This requires ASI Loader.

---

If you want complete package for easy installation, that includes all aforementioned fixes and [Ultimate ASI Loader](https://github.com/ThirteenAG/Ultimate-ASI-Loader) as **XLiveLess**, plus [XLiveLessAddon](https://bitbucket.org/ThirteenAG/xlivelessaddon/downloads/) to make the game work without xlive,

### **Download**: [GTAIV.EFLC.FusionFix.Mid.zip](https://github.com/ThirteenAG/GTAIV.EFLC.FusionFix/releases/latest/download/GTAIV.EFLC.FusionFix.Mid.zip)

---

If you want to install other mods along the way, including all aforementioned fixes, [Ultimate ASI Loader](https://github.com/ThirteenAG/Ultimate-ASI-Loader) as **XLiveLess**, plus [XLiveLessAddon](https://bitbucket.org/ThirteenAG/xlivelessaddon/downloads/) to make the game work without xlive, [ColAccel](https://github.com/ThirteenAG/IV.EFLC.ColAccel), a plugin that reduces loading times, [Project2DFX](https://github.com/ThirteenAG/III.VC.SA.IV.Project2DFX), a plugin that adds lod lights,

### **Download**: [GTAIV.EFLC.FusionFix.Max.zip](https://github.com/ThirteenAG/GTAIV.EFLC.FusionFix/releases/latest/download/GTAIV.EFLC.FusionFix.Max.zip)

---

Unpack the content of archive to your **GTAIV** or **EFLC** directory.

**TBoGT as DLC note**: if you have episodes installed as DLC in your **GTAIV** folder, you need to move

**Grand Theft Auto IV/TBoGT/pc/models/cdimages/vehicles.img**

to

**Grand Theft Auto IV/DLC/TBoGT/content/pc/models/cdimages/vehicles.img**

---

## Files rundown:

    TBoGT/pc/models/cdimages/vehicles.img

**Car lights fix for TBoGT.**

    pc/data/maps/props/vegetation/ext_veg.ide
    pc/data/maps/props/vegetation/ext_veg.img

**Trees shadows fix.**

    common/shaders/win32_30/gta_emissivestrong.fxc
    common/shaders/win32_30_atidx10/gta_emissivestrong.fxc
    common/shaders/win32_30_low_ati/gta_emissivestrong.fxc
    common/shaders/win32_30_nv6/gta_emissivestrong.fxc
    common/shaders/win32_30_nv7/gta_emissivestrong.fxc
    common/shaders/win32_30_nv8/gta_emissivestrong.fxc

**Corrected shaders to make the lights appear. Used in conjunction with GTAIV.EFLC.FusionFix.asi.**

    plugins/GTAIV.EFLC.FusionFix.asi
    plugins/GTAIV.EFLC.FusionFix.ini

**Recoil, definition and shader bugs are fixed here.**

# Reporting more issues

We're making a list of **GTA IV** issues that weren't addressed in official patches.

If you can think of one, submit it [here](https://github.com/GTAmodding/GTAIV-Issues-List/issues).

If you've encountered an issue, caused by this fix, report it [here](https://github.com/ThirteenAG/GTAIV.EFLC.FusionFix/issues).
