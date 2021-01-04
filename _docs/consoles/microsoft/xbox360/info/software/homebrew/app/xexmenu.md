---
title: XeXMenu
description: Xbox 360 homebrew file manager
tags:
 - consoles
 - microsoft
 - xbox360
---

# XeXMenu

XeXMenu is a file manager for the Xbox 360. 

### It is recommended to install this app on a RGH/JTAG. Though limited in function as a Dashboard, it is a powerful standalone file manager.

A video tutorial on Installing XeXMenu can be found by [MrMario2011](https://www.youtube.com/watch?v=w5xVFNkxv-I) or [Modded Warfare](https://www.youtube.com/watch?v=eq-ky8T6kl4).

- The default username/password for FTP is "xbox" and "xbox".
- This cannot be changed in the configuration.

------

## Installation

You will need:

- A console capable of running unsigned code
- [A copy of XexMenu](https://mega.nz/file/9AlUmDZK#oykniipcx80kvuRxLaqY8NtPMJYKHW1ZYpqYfcAZsLA) [Alt Download](http://www.mediafire.com/file/7orm0jrkncrzo1w/xexmenu12live.rar/file)
- A method to transfer files to the Xbox 360 from your PC

Installation:

1. Plug a flash drive into your Xbox 360 and navigate to Console Settings > Storage. Select the flash drive and allow it to format the flash drive as a system drive. 
2. Extract the `CODE9999` folder from the `XeXMenu 1.2 rar` archive to the `Content/0000000000000000/` folder on your Xbox 360/USB.
3. Navigate to the Demos section of the stock dashboard and launch XeXMenu from there.
   - You can install XeXMenu to your hard drive by going to Console Settings > Storage, and copying it from your flash drive to the hard drive.

## Controls

- **Back**: Visual control list
- **Start**: Launch selection
- **LB**/**RB**: Change menu
- **D-PAD Left**/**Right**: Change tab
- **Y**: Rescan devices / file context menu
- **A**: Launch selection
- **B**: Back (in file manager)

## Discovery Menu

### Games Discovery

- Games in `hdd1://Games` will be listed here and launchable. 
- Press **left**/**right** on **D-PAD** to change to a different tab.

### Emulators Directory

- Emulators in `hdd1://Emulators` will be listed here and launchable. 
- Press **left**/**right** on **D-PAD** to change to a different tab.

### Applications Directory

- Executables in `hdd1://Apps` will be listed here and launchable. 
- Press **left**/**right** on **D-PAD** to change to different directory.

## File Manager Menu

- Files and folders are listed for the selected device.
- Change selected device tab by pressing **X** and selecting a device with **A** or press **left**/**right** on **D-PAD** to cycle through available device tabs.
- **Do not touch the files in Flash unless you know what you are doing. These are system files and you can brick your system requiring the NAND to be rewritten.**
- Press **Y** to open the context menu on any file/folder for Copy, Paste, Cut, Delete, CopyDVD, PatchXex, and Create options.

### CopyDVD

- Copies the contents of the inserted DVD to the current directory in the file manager. [More information can be found in the Xbox 360 ripping guide]({{ site.baseurl }}/docs/consoles/microsoft/xbox360/guides/mod/backups/games/ripping).

### PatchXex

This option will patch games to run from your hard drive instead of DVD. [You can learn more in the Xbox 360 HDD game patching guide]({{ site.baseurl }}/docs/consoles/microsoft/xbox360/guides/mod/patching/games/runfromhdd).

## Configuration

- **Skin**: Allows you to change the XeXMenu skin. By default, there are 26 skins installed.
- **Enable skin auto scaling**: Resizes the skin to fit your TV
- **Auto extract games title**: Uses the official game title from the XEX of the game instead of the filename
- **Discover only default.xex**: Only shows default.xex files in the file discovery menus, ignoring any XEX not named "default".
- **Sensor**: Displays CPU/GPU/EDRAM/Motherboard temperatures.
- **SMC Version**: Shows the System Management Controller version.



# References

https://www.reddit.com/r/360hacks/wiki/xexmenu - Thanks to the 360hacks wiki team for their work!

