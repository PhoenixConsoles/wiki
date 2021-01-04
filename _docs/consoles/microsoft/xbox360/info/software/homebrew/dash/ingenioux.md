---
title: IngeniouX Dashboard
description: Xbox 360 homebrew dashboard IngeniouX
tags:
 - consoles
 - microsoft
 - xbox360
---

# IngeniouX

------

[IngeniouX](http://www.mediafire.com/file/3hzk7vcoqpfgqmk/ingeniouxb3.rar/file) is a custom dashboard that is able to launch game backups, use FTP, use dashboard skins, and manage files. It also includes a built in  calculator and MP3 player. 

- The default username/password for FTP is "xbox" and "xbox".

------

## Installation

Extract the files from `ingeniousxb3.rar` and copy them to your Xbox 360. Use a file manager to launch the .xex.

## Controls

- **A**: Enter/confirm/launch
- **B**: Back
- **Y**: Context menu
- **X**: Select multiple in file browser
- **LB/RB**: Change menu
- **LS**: Open On-board apps menu
- **DPAD**: Movement

## Launching Games

Depending on whether your game was downloaded from Xbox Live or  ripped from a disc, it will show up in the respective tab for  "Downloaded Content" or "Extracted DVD Game". Launch it by pressing A.

## Extracting Cover Art

By hovering over a game and pressing Y, you have the option to  extract artwork directly from the game. Not all games have extractable  artwork, but the options are as follows:

- **Extract HD Picture**: This will extract a HD picture from the game and place it in the Wallpapers section of the dashboard.
- **Extract Preview**: This will extract a picture from the game that will be placed in the box on the right hand side of the game launcher.
- **Extract Icon**: This will extract the game icon and display it to the left of the game title.

Press Y and Refresh to accept changes.

## File Browser

The file browser is a standard commander-style file manger. You can  press Y to open the context menu on a file/folder to  Copy/Move/Rename/Delete, or create a folder (create archive is not  available). Press X to select multiple files or folders.

## Options

- **Skin**: Allows you to apply a skin that you've placed in .../IngeniouX/Skin.
- **Game Folder**: Lists the directories being searched for games. You can change this by changing the paths in .../IngeniouX/config.ini
- **Language**: Allows you to change the dashboard language. Due to a bug, you will need to choose the language *above* your desired language.
- **Wallpaper**: Allows you to apply a wallpaper  supplied by extracting it out of a game in the game launcher, or by  placing a picture in the ,,,/IngeniouX/Wallpaper folder.
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
- Horizontal/Vertical overscan settings appear to be brokens