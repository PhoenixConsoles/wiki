---
title: IngeniouX Dashboard
description: Xbox 360 homebrew dashboard IngeniouX
tags:
 - consoles
 - microsoft
 - xbox360
---

# IngeniouX

### It is not recommended to use IngeniouX. It is not as fully-featured as other dashboard replacements and is buggy.

IngeniouX is a custom dashboard that is able to launch game backups, use FTP, use dashboard skins, and manage files. It also includes a built in calculator and MP3 player. 

- The default username/password for FTP is "xbox" and "xbox".

------

## Installation

You will need: 

- [A copy of IngeniouX](http://www.mediafire.com/file/3hzk7vcoqpfgqmk/ingeniouxb3.rar/file).
- [XexMenu]({{ site.baseurl }}/docs/consoles/microsoft/xbox360/info/software/homebrew/app/xexmenu)
- A method to transfer files from your PC to your Xbox 360

Instructions:

1. Extract the files from `ingeniousxb3.rar` and copy them to your Xbox 360's `Apps` folder. The resulting file structure should be `Apps/IngeniouX/` on the Xbox 360.
2. Launch the .xex from the `IngeniouX/` folder in `Apps`.
3. (Optional) Set the .xex from step 2 to default in [DashLaunch]({{ site.baseurl }}/docs/consoles/microsoft/xbox360/info/software/homebrew/app/dashlaunch)

## Controls

- **A**: Enter/confirm/launch
- **B**: Back
- **X**: Select multiple in file browser
- **Y**: Context menu
- **LB/RB**: Change menu
- **Left Stick**: Open On-board apps menu
- **D-PAD**: Movement

## Launching Games

If your game was downloaded from Xbox Live it will show up in the "Downloaded Content" tab, if it is a ripped game then it will show up under the "Extracted DVD Game" tab. Launch it by pressing **A**.

## Extracting Cover Art

By pressing **Y** while selecting a game, you have options to extract artwork directly from the game.

- **Extract HD Picture**: This will extract a HD picture from the game and place it in the Wallpapers section of the dashboard.
- **Extract Preview**: This will extract a picture from the game that will be placed in the box on the right hand side of the game launcher.
- **Extract Icon**: This will extract the game icon and display it to the left of the game title.

Press **Y** and refresh to accept changes.

*Not all games have extractable artwork*

## File Browser

- Commander-style file manager.
- Press **Y** to open the context menu on a file/folder to Copy/Rename/Delete/Move or to create a folder. Creating archives is unavailable.
- Press **X** to select multiple files/folders.

## Options

- **Skin**: Allows you to apply a skin that you've placed in `IngeniouX/Skin`.
- **Game Folder**: Lists the directories being searched for games. You can change this by changing the paths in `IngeniouX/config.ini`.
- **Language**: Allows you to change the dashboard language. Due to a bug, you will need to choose the language *above* your desired language.
- **Wallpaper**: Allows you to apply a wallpaper supplied by extracting it out of a game in the game launcher, or by placing a picture in the `IngeniouX/Wallpaper/` folder.
- **H-ov**: Horizontal overscan (not functional)
- **V-ov**: Vertical overscan (not functional)
- **Show Log**: ??? - To get to this option, scroll to the bottom of the Language window and press down once more. Press A to toggle.

## On-Board Apps

- **Text Viewer**: Used to view text.
- **Image Viewer**: Used to view images. 
- **Archive Manager**: Not implemented.
- **Calculator**: A simple calculator.
- **MP3 Player**: Designed to play music.

## Bugs

- FTP, Text Viewer, and Image Viewer appears to be broken in Beta 3.
- MP3 Player crashes if you press any of the player buttons without any music installed. Playlists are not saved.
- Image extraction can take a few minutes and sometimes does not extract anything at all.
- The language selection suffers from an "off by one" programming error, so you will need to choose the language *above* your desired language in order to apply it.
- Horizontal/Vertical overscan settings appear to be non functional

# References

https://www.reddit.com/r/360hacks/wiki/ingenioux - Thank you to the 360hacks wiki team for their work!

