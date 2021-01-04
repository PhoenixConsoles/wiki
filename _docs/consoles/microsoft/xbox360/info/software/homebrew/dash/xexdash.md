# XexDash

Not to be confused with [XexMenu]({{ site.baseurl }}/docs/consoles/microsoft/xbox360/info/software/homebrew/app/xexmenu).

### It is not recommended to use XeXDash, as it is outdated and not as feature-complete as other options.

XexDash is a minimal dashboard replacement capable of launching game backups, FTP, and changing fan speeds. On release, XexDash was used for supporting Chinese and Japanese characters in game and folder names, a feature that caused issues on other dashboards.

- The default username/password for FTP is "xbox" and "xbox".
- If you have issues using FTP after using this dashboard, delete the `XexDash.xml` file it generated on hdd1:. You may need to completely remove the dashboard and restart your Xbox 360 to get it to work. 

------

## Installation

### As a Demo Shortcut

1. Extract XexDash_Dashboard.zip and copy the folder `C0DE0003` to `Hdd1:\Content\0000000000000000` or `usb1:\Content\0000000000000000`. 
2. Launch it from the Microsoft dashboard by navigating to Game Library > Demos > XexDash.

### As a XEX

1. Extract XexDash_Xex.zip and copy the folder "XexDash" to your Xbox 360's `Apps` folder. 
2. Use a file manager to navigate into the folder and launch it by selecting the .xex,
3. (Optional) Set the .xex from step 2 to default in DashLaunch.

## Controls

- **D-PAD**: Up/down/left/right
- **LT**/**RT**/**LB**/**RB**: Page up/down on games
- **A**: Enter/Confirm
- **Y**: Menu
- **X**: Sort games by name
- **B**: Readme
- **Back**: Return to Dashboard

## Game Launcher:

1. Copy your game files of an Xbox or Xbox 360 game to a folder inside of `Hdd1:\hidden`, `Usb0:\hidden`, `Cdrom0:\hidden`, or `Devkit:\hidden`. 
2. From the main screen of XexDash, press Y to open the menu, then select Driver Disk, and choose the device holding the game files. It will populate a list of your games. 
3. Hover over a game and it will list the title ID in the top left of the screen, and you can launch it by pressing A. 

- If you wish to add cover art to the game, place a picture named `default.png` in the game folder and it will display in the bottom left corner.

## FTP Server

- Your IP is listed in the bottom right of the screen. 
- You can connect to it at port 21 with the username `xbox` and password `xbox`. 

## Menu

- **Driver Disk**: Selects the device to load the game list from.
- **Type**: Change the type of game to regular game or XBLA game.
- **Language**: Change the language to English, Japanese, or two dialects of Chinese.
- **Set**: Press left or right on the DPAD to select where it pulls a background image from. The easiest way is to set it to [system] and place a `background.jpg` in `XexDash/media/`.
- **Update**: Previously would update the dashboard. No longer functional.
- **Fan**: Press left or right on the DPAD to change the fan speed by 5%. Setting applies from when you open XexDash until Xbox is shut off.
- **Return to XDK**: Returns to the XDK menu, or if not installed, your default dashboard.
- **Return to Dash**: Returns to your default dashboard.