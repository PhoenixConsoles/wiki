---
title: X360DebuggerWV
description: Xbox 360 official networking tool for developers
tags:
 - consoles
 - microsoft
 - xbox360
---

# Xbox 360 Neighborhood

Xbox 360 Neighborhood is an official SDK tool created by Microsoft for use with development kits. The tool can also be used with RGH/JTAG exploited consoles. Xbox 360 Neighborhood is often used by modders as it provides a simple integration of your console into your PC and network.

## Features

- Basic FTP
- Live Peeking/Poking of values in RAM
- Running executable XEX files remotely

Video tutorials on installing and using Xbox 360 Neighborhood are available from [Modded Warfare](https://www.youtube.com/watch?v=aqmO-T7LlTc) and [XeXSolutions](https://www.youtube.com/watch?v=Vjp-PHwMh6U)

**Note: Since Xbox Neighborhood is an official Microsoft tool, it can not be distributed. Do not ask for download links.**

## Installing

You will need: 

- An Xbox 360 development kit or RGH/JTAG retail.
- A Windows PC
- A copy of the Xbox 360 SDK
- XBDM

Instructions:

1. (Optional) Install the Visual Studio 2010 Ultimate edition
2. Install Neighborhood and (Optionally) the Xbox 360 SDK full version.
3. Load up Xbox 360 Neighborhood.

## Adding a Console

1. Place xbdm.xex on the root of `HDD1:`. If the file `xbdm.ini` is present, delete it.
2. Reboot your console, and launch Xbox 360 Neighborhood on your PC.
3. If not automatically prompted, select "Add Xbox 360".
4. Enter the console name (default "Jtag") or the IP address. It will add the console into your Xbox 360 Neighborhood window.
   - You can change the icon and name by editing the "xbdm.ini" file that is generated in the root of HDD1. Valid names are `black gray blue white nosidecar`.

## Taking a Screenshot

To take a screenshot, simply right-click your console and select "Screen capture".

## Executing an XEX

Double-click on your console to browse its files. Locate the XEX you want to launch and double click it.

## Troubleshooting

- Hang/Crash
  - Crashes are inevitable in Xbox Neighborhood. When they happen, they  will also crash explorer.exe, the interface of Windows. To restore  explorer.exe, press Win+R and type "explorer.exe" and press Enter. You  can prevent it from crashing explorer.exe on Windows 7, by opening File  Explorer, pressing Alt > Tools > Folder Options > View, and  ensuring "Launch folder windows in a separate process" is checked. If  not, change it and press Apply. By default, Windows 10 has this option  checked.



# References

Thanks to Modded Warfare and XeXSolutions for their videos.

https://www.reddit.com/r/360hacks/wiki/xbox_neighborhood - Thanks to the 360hacks wiki team for their work!

Thanks to Microsoft for creating this wonderful tool!