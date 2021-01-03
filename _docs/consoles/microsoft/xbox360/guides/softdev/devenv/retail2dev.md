---
title: Setting up a Xbox 360 Development Environment
tags: 
 - xbox360
 - xbox360dev
 - xbox
 - dev
 - modding
 - xbox360modding
description: Setting up a Xbox 360 Development Environment


---

# 

# Convert Retail Console to Devkit Console

Converting a retail console to a development console will help you work on developing homebrew software for the Xbox 360 by providing a test environment which streamlines the development process by allowing access to SDK[LINK NEEDED] features unavailable via Freeboot[LINK NEEDED] or stock NAND. This is done using RGLoader[LINK NEEDED], which is a tool that can build a devkit NAND from a retail NAND dump. The devkit NAND enables debug features not otherwise available on a modified console capable of running unsigned code. This process also installs xshell[LINK NEEDED], the official development dashboard[CITATION NEEDED].



## WARNINGS

- Doing this should increase performance with Xbox 360 Neighborhood[LINK NEEDED].[CITATION NEEDED]
- This is **NOT** for people who aren't looking to get into development for the Xbox 360.
- The latest kernel available for this is **NOT** the latest kernel. It is currently on `17150`[CITATION NEEDED]. This means you *will not* be able to go on Xbox Live with RGLoader[CITATION NEEDED]. 
- You will be unable to play system link[LINK NEEDED] with anyone who does not have either a devkit[LINK NEEDED] or the devkit patch enabled in DashLaunch[LINK NEEDED].
- You will be able to do everything you could with a Freeboot[LINK NEEDED] NAND.
- This can go wrong and brick your console. JTAGs[LINK NEEDED] are especially common to brick.[CITATION NEEDED]
- RGLoader[LINK NEEDED] overwrites XeLL[LINK NEEDED], therefore the only way to revert this is to reflash the NAND[LINK NEEDED] with the XeLL[LINK NEEDED] or stock image[LINK NEEDED].

- Dashlaunch does not work with a devkit NAND.[CITATION NEEDED]
- Fakeanim does not work with a devkit NAND. You will have to remove the `;` and edit the path to your fakeanim in rgloader.ini if you wish to use it.[CITATION NEEDED]
- By default it will boot into the xshell[LINK NEEDED] dashboard. You can change this by changing the path to a different dashboard's XEX in rgloader.ini
- You must remove your xbdm.ini file from your console or you will be stuck on the Xbox loading screen.
- If when you boot into RGLoader where it is in "minimal mode" where you cannot boot into games, the dashboard, etc., ensure your system is set up correctly.
- If there are two CPU_Key lines in `options.ini`, remove one of them.
- On first boot, it may take a while as it is setting up.
- Sometimes it will appear to be in minimal mode, but functionality will work fine regardless.
- For network setup, you may need to enter xshell[LINK NEEDED], go to Tools > Network Settings > Debug configuration, and set Configure IP to `Manual` and then back to `Automatic` if it does not get a valid IP.
- Devkit profiles and Retail profiles are different and not cross-compatible without the `devprof` setting enabled in DashLaunch, which allows Freeboot NANDs to use devkit profiles. Retail profiles will not appear in devkits and devkit profiles will appear corrupted on retail consoles without that setting enabled.
- RAM dumps[LINK NEEDED] are much faster with RGLoader than with xbdm.xex[LINK NEEDED].[CITATION NEEDED]
- You can use XBMovie[LINK NEEDED] to record the screen for short periods of time.[CITATION NEEDED]

## You will need:

A modified retail console capable of running CFW[LINK NEEDED]

A copy of RGLoader[LINK NEEDED]

## How to do it

1. Acquire a dump of your NAND.[LINK NEEDED]
2. Transfer the `Filesystems` folder, `rgloader.ini` to your hard drive(HDD:). This is **case-sensitive**.
3. You will edit the options.ini file to replace the CPU_Key field with your cpukey. Learn how to find your CPU Key here[LINK NEEDED]. Replace the exploit field with the exploit type for your console. Replace the kernel field with the kernel of your choice available in the `Filesystems` folder.
4. Open `RGBuild Launcher` and confirm the information is correct.
5. Select NAND and open the dump of your NAND. This will create the RGLoader[LINK NEEDED] devkit NAND.
6. Flash the RGLoader NAND to your console[LINK NEEDED].
7. Select your language for xshell[LINK NEEDED]. Then choose a machine name. Congratulations, you're all done!



## See also

Xbox 360 Neighborhood[LINK NEEDED]

XBMovie[LINK NEEDED]

## References

[Modded Warfare for their tutorial on turning a JTAG/RGH into a DevKit with RGLoader.](https://www.youtube.com/watch?v=YeFZd6R3K90)