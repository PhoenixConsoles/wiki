---
title: XCE Tools
description: Xbox 360 remote debugger for scanning memory ranges to find offsets of specific values.
tags:
 - consoles
 - microsoft
 - xbox360
---

# XCE Tools

------

XCE Tools is a debugger similar to Cheat Engine on PC. A highly helpful tool for making mod menus, cheats, or patches for games.

### Features

- Scan memory ranges
- Find offsets of specific values

## Setup

You will need:

- [A copy of XCETools](https://mega.nz/file/Jd4i0LqL#vUJWHOphPSOK9unwqJranCsau2nL1zjpbo93xRcCTr4)
- JRPC/XRPC
- RPC
- XBDM

Instructions

1. Transfer JRPC/XRPC, RPC, and XBDM to the root of the Xbox 360.
2. Plugins should be set as follows
   1. XBDM
   2. RPC
   3. JRPC
3. Reboot the Xbox 360 and confirm connectivity with Xbox 360 Neighborhood.
4. Connect to the Xbox 360 with XCETools.

## Usage Example

This example is a hypothetical example using the game Doom 3. In this example, we will set the health counter to 900%.

1. Verify Xbox 360 Neighborhood is connected, then launch  XCE_Tools2.exe. Launch your game of choice and progress through the game until you reach a point in which you can visually see your value, for  instance a health counter. If possible, try and make this value a number that is not `0` or `1` as these are extremely common values and may take longer to find. For this example, we will say the health counter is at 57%.
2. In XCE Tools, change the value of the second Range field to `D0000000`. This will reduce the number of RAM addresses that it will search to a  range that your target value (in this example, our health counter) is  more likely to be in.
3. If your number can only be an integer with no decimal points,  select the "4 bytes" checkbox at the top and the "4 bytes" radio button  on the right side. Otherwise, select "float" or "double". It is  partially guess work as to which type your value is, and it will help  you to look up what the maximum value each type can represent. For this  example, we know that our number goes up to 200 normally, so it is  likely a 2 byte or 4 byte number. We will choose 4 bytes as it is more  common.
4. If possible, pause your game so that less things are being processed and less values are changing in RAM.
5. Click the Init button. The program will begin dumping the RAM of  your console and show a progress bar in the bottom left. The process  will take quite a while. Do not use your console while this is dumping,  as you may inadvertently change the value you are trying to find.
6. In the field next to the "Exact" button, enter the target value  that you are trying to find an address for (in this example, 57) and  press the Exact button. This will remove all values from the RAM dump  that don't match your target value and list the address offsets that  match your value.
7. Do something in-game that will cause your target value to change. Repeat step 6 using the new target value. In this example, we will take damage and the health counter will end up at 62%, so we will input 62.  This will take the list of addresses that had previously had the value `57` and will remove the ones that did not change to `62`. Repeat this process until you are only left with a very small amount (1 to 5) values. In this example, lets assume we are left with:
   - 001: ABCD1234: 57>>62
   - 002: AAAA1234: 57>>62 
   - 003: DAAD0000: 57>>62
8. The offset we want is one of these. Often times multiple offsets  follow the same path of changes as it might be separate variables for  displaying graphics or just a copy of the variable. The only way to  really know for sure which value is the one we want is to manually  change (poke) the value and see if it changes in-game. For this, we can use [Peek Poker](peekpoker).



## Bugs

- If you  have more than one monitor plugged in then the program will not start  properly. However it seems to run fine if you start the program with  only one display then connect more afterwards. Very weird. It does work with multi-monitors but if you  have a laptop the primary display in Windows must be set to the built in laptop display.

# References

https://www.reddit.com/r/360hacks/wiki/xce - Thanks to the 360hacks wiki team for their work!

The creator of XCETools. If you know any more please submit the information!