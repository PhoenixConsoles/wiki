---
title: Peek Poker
description: Xbox 360 remote debugger for viewing and modifying values in RAM
tags:
 - consoles
 - microsoft
 - xbox360
---

# Peek Poker

Peek Poker is a tool used to view and modify values in live RAM on an Xbox 360.

## Setup

You will need:

- [A copy of Peek Poker](https://github.com/360Haven/PeekPoker)
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
4. Connect to the Xbox 360 with Peek Poker.

## Usage Example

- This example assumes that you have used another tool, such as [XCE Tools](xcetool) to find the offsets for a value you wish to change in-game. This provided example continues the example found on the XCE Tools page which we are trying to change the target value to 900, and we had found the potential offsets for the target value as:
  - 001: ABCD1234: 57>>62
  - 002: AAAA1234: 57>>62 
  - 003: DAAD0000: 57>>62

1. Enter your Xbox 360's IP address into Peek Poker and click Connect. 
2. Click the "Peek & Poke" button. Enter the address of the first offset (in this example, ABCD1234) and press the Peek button. This will pull up the location in RAM that the value resides in. In this example, it will still have the value of 62 represented in hexidecimal (3E). 
3. Select the found value (in this example, 3E) and change it to another hexidecimal value such as 63 (900 in decimal) and press the Poke button. If your game is paused, unpause it and see if the value in-game changed as expected. If not, try another potential offset (in this example, AAAA1234 or DAAD0000). Sometimes, one of these offsets may visually change the display, but not actually change the value in-game. In this example, the first offset may change the displayed health counter value, but in reality, you still have low health and will die quickly if you take damage. Because of this, you should Poke an offset and test to make sure it behaves as intended and not just rely on visual changes.

- Note that not all games use static offsets, and the offsets may change every time you restart the game. If you plan on making a mod tool, reboot your console and verify that you can still poke the same offset and get the same results.



# References

https://github.com/360Haven/PeekPoker - Thanks to 360Haven for this open source tool!

https://www.reddit.com/r/360hacks/wiki/peekpoker - Thanks to the 360hacks wiki team for their work!

