---
title: DashLaunch
description: Xbox 360 homebrew utility for deep system configuration
tags:
 - consoles
 - microsoft
 - xbox360
---

# DashLaunch

DashLaunch is a tool for tweaking deep system settings. **You must save your changes if you make any modifications.**

### It is recommended to install this app on a RGH/JTAG. Though limited in function as a Dashboard, it is a powerful configuration manager.

- The default username/password for FTP is "xbox" and "xbox".
- This can be changed through the configuration menu.

Video tutorials on installing and configuring DashLaunch are available from [Modded Warfare](https://www.youtube.com/watch?v=y2zCQD0RaeA) and [XeXSolutions](https://www.youtube.com/watch?v=OJcHQUk9S20)

## Installation

You will need:

- [DashLaunch](https://www.mediafire.com/file/3dalys9jh2ymbjy/dash_launch_v3.19.zip/file)
- [XeXMenu]({{ site.baseurl }}/docs/consoles/microsoft/xbox360/info/software/homebrew/app/xexmenu)
- A console capable of running unsigned code.
- A method of transferring files from PC to Xbox 360.

Instructions:

1. Extract DashLaunch and copy the files to the `Apps` folder so the resulting file tree is `Apps/DashLaunch/`.
2. Open XeXMenu and browse to the `Apps/DashLaunch/` folder.
3. Launch the xex.
4. Configure your `launch.ini` through the interface and [save it using the Save / Load Options tab](#save-load-launchini).

## Controls

- **Back**: Display controls
- **B**: Quit back to main dashboard
- **Y**: Clear path (if hovering on path setting)
- **LB/RB**: Change menu
- **LT/RT**: Jump to top or bottom of current page view.
- **D-PAD Up**/**Down**: Move up or down

## Menu

### Current Options

#### Paths

- **dumpfile**: Location to save a crash dump file if your system crashes. It's recommended to set this so that you can troubleshoot your system in the future.
- **Default**: Path to the XEX (usually a dashboard) you want to launch automatically at startup. If nothing set, it will boot the original dash.
- **(buttons)**: Path to the XEX you want to launch automatically at startup or when you if you are holding the listed button. If nothing set, it won't do anything. RB will always go to the default dashboard.
- **configapp**: Path to the XEX you want to launch when you select System Settings from the miniblades. Nosysexit must be disabled under Behavior.
- **Guide**: Path to the XEX you want to launch when you turn on the console with the guide button.
- **Power**: Path to the XEX you want to launch when you turn on the console with the power button.
- **Fakeanim**: Replaces the boot animation with a custom one. This animation plays before any other of the above options are processed.

#### Behavior

Recommended settings are in brackets next to the option name.

- **contpatch [enabled]**: When enabled, DLC and addons will work without proper licensing.
- **xblapatch [enabled]**: When enabled, XBLA games will boot without proper licensing. 
- **licpatch [enabled]**: When enabled, extracted XBLA games will boot without proper licensing.
- **nxemini [enabled]**: When enabled, pressing Y while the miniblades menu is open will launch whatever is set in the Default path option.
- **dvdexitdash [disabled]**: When enabled, pressing Eject will return you to the official dash.
- **xblaexitdash [disabled]**: When enabled, exiting an XBLA game through its menu will return you to the official dash.
- **nosysexit [disabled]**: When enabled, System Settings in the miniblades will launch what is set in the configapp path. If nothing is set, System Settings will do nothing.
- **nohud [disabled]**: When enabled, the miniblades option will not pop up when you press the Guide button.
- **nohealth [enabled]**: When enabled, the Kinect health video at the start of Kinect games will not be shown.
- **noobe [enabled]**: When enabled, prevents dash locale setup screen from showing when dash starts. 
- **autoswap [disabled]**: When enabled, DashLaunch will perform automatic disc swapping for multi-disc games. **Do not enable this if using FSD or swap.xex**.
- **regionspoof [enabled]**: When enabled, holding RB while launching a game will cause the region to be spoofed.
- **region [default]**: Region to be spoofed to when regionspoof is enabled. 0x7FFF (DEVKIT/ALL) is enabled by default.
- **autoshut [enabled]**: When enabled, pressing the Guide button will automatically highlight "Turn Off Console" instead of Cancel. 
- **autooff [disabled]**: When enabled, automatically shuts off the console when the Guide button is held. Automatically overrides autoshut.
- **shuttemps [disabled]**: When enabled, if you hold the Guide button, the temperatures captured at that moment will be displayed on the shutdown scren. This disables autooff.
- **devprof [enabled]**: When enabled, profiles from a devkit will not appear as corrupt.
- **fatalreboot [disabled]**: When enabled, console will hard reboot if it crashes. Recommended to be disabled in case there is a ROL error code.
- **fatalfreeze [disabled]**: When enabled, console will freeze if it crashes. Disables fatalreboot.
- **safereboot [disabled]**: When enabled, console will soft reboot on fatal crashes. Do not use on JTAG, as it will show an E79 error unless you used the transistor method for the JTAG install. 
- **exchandler [enabled]**: When enabled, non-fatal crashes will exit instead of crashing the console.
- **debugout [enabled]**: When enabled, debug messages are sent to UART.
- **passlaunch [disabled]**: When enabled, DashLaunch will not delete your recent played icons.
- **noupdater [enabled]**: When enabled, your console will look for system updates named $$ystemUpdate instead of $SystemUpdate. This prevents accidental updates, as you would have to rename the folder yourself to apply an update.
- **remotenxe [disabled]**: When enabled, powering on the console with an IR remote will go to the official dash. 

#### Network

Recommended settings are in brackets next to the option name.

- **pingpatch [enabled]**: When enabled, the 30ms ping limit is removed for sysem link. This is useful for Xlink Kai and other network tunnels.
- **signnotice [enabled]**: When enabled, sign in messages will be suppressed. 
- **liveblock [enabled]**: When enabled, known Xbox Live sites are blocked. Xbox Marketplace data can still be accessed. 
- **livestrong [enabled]**: Requires liveblock to be enabled. When enabled, all Xbox Live sites are blocked, including Xbox Marketplace data sources.
- **xhttp [disabled]**: When enabled, patches XAM to allow insecure access from other devices. Having this option enabled may cause issues with mod menus.
- **nonetstore [enabled]**: When enabled, cloud storage does not show up in storage selection screens.
- **devlink [disabled]**: When enabled, system link data will be encrypted for connection with developer consoles. This may negatively impact Xlink Kai if it is enabled.
- **sockpatch [disabled]**: (description pending)
- **fakelive [disabled]**: When enabled, fakes an Xbox Live connection for all apps and games, which allows you to access Live-only menus. This causes issues with many games.
- **autofake [enabled]**: When enabled, automatically fake an Xbox Live connection for indie games and the official dash. Without it, you cannot play indie games.
- **autocont [disabled]**: When enabled and contpatch is disabled, it will temporarily enable contpatch to launch indie games. This will enable autofake.
- **autofake# [disabled]**:When enabled, fakelive will be temporarily enabled when the specified TitleID is launched.

#### Timers

Recommended settings are in brackets next to the option name.

- **hddtimer [default]**: When hddalive is enabled, this sets how often DashLaunch will poll the USB drives for device changes.
- **hddalive [disabled]**: When enabled, any USB drive containing "alive.txt" in its root directory will be polled at the interval set in hddtimer to keep it awake. 
- **temptime [default]**: Frequency at which temperature info is updated in DashLaunch.
- **tempport [disabled]**: Network port that the temperature information will be broadcast on when tempbcast is enabled.
- **tempbcast [default]**: When enabled, system will broadcast temperature information on the network on the port specified by tempport.

#### Plugins

- Allows you to set plugins at the specified paths to be launched at startup. Press Y to clear line and stop a plugin from launching. 

#### Configurator

Recommended settings are in brackets next to the option name.

- **ftpserv [disabled]**:When enabled, a FTP server will run when DashLaunch is running. Takes effect after reboot.
- **ftpport [default]**: Port at which an FTP server will run while in DashLaunch. Requires ftpserv to be enabled.
- **updserv [disabled]: When enabled, starts a server which you can connect to for updating your XeBuild image.
- **calaunch [disabled]**: When enabled, DashLaunch will start on the Launch menu instead of Current Options.
- **fahrenheit [disabled]**: When enabled, system temperatures in DashLaunch will be shown in Fahrenheit instead of Celsius. It is recommended to leave it in Celsius, as that is the setting most temperature baselines are based off of.

### Save \ Load launch.ini

This menu allows you to load (A), delete (Y), or save (X) a launch.ini config. To save the config, highlight the desired location to save it to, and press X. It is recommended to save config files to Flash to have them run at startup.

### Miscellaneous

- **Launch**: Allows you to browse for and launch an XEX.
- **System Info**: Shows system info such as your serial number and CPU key.
  - **SMC Config Settings**: This section allows you to change the target temperature for your CPU, GPU, and EDRAM. This setting is active regardless of what dashboard or app/game you are in. The optimal value is different per system, but it's generally recommended to choose target temperatures below 70°C that don't run the fan too loudly. You can also set the fan at a certain percent instead with the fan override settings, but this is not recommended as it does not account for the varying temperatures that occur during use.
- **Load/Unload DashLaunch**: Loads or unloads DashLaunch from memory.
- **Install/Uninstall**: Installs or removes DashLaunch from system flash.
- **Update Patches**: Forces DashLaunch to patch and update.
- **Install This**: Copies DashLaunch to the folder you choose.
- **Quit**: Returns to the default dashboard.

# References

https://www.reddit.com/r/360hacks/wiki/dashlaunch - Thanks to the 360hacks wiki team for their work!