---
title: Aurora Dashboard
description: Xbox 360 homebrew dashboard, .
tags:
 - consoles
 - microsoft
 - xbox360
---

# Aurora Dashboard

[Aurora](http://phoenix.xboxunity.net/#/news) [[Archive.org]](https://web.archive.org/web/http://phoenix.xboxunity.net/#/news) is a homebrew dashboard replacement, whos design is centered around the colorful coverflow design of its game launcher. Features include customizable skins, automatic download of title updates and cover art, the ability to organize games into categories, FTP support, integrated XLink Kai, screenshots, a http server, temperatures in the blades guide, and a plugin system. 

It is the most recently updated homebrew dashboard replacement, with an official website at [XboxUnity.net](http://xboxunity.net) [[Archive.org]](https://web.archive.org/web/http://xboxunity.net) and an official support forum at [RealModScene.com](https://www.realmodscene.com/) [[Archive.org]](https://web.archive.org/web/https://www.realmodscene.com/). An FAQ can be found [here](https://www.realmodscene.com/index.php?/topic/5851-useful-qa-for-new-people-faq/) [[Archive.org]](https://web.archive.org/web/https://www.realmodscene.com/index.php?/topic/5851-useful-qa-for-new-people-faq/).

A video walkthrough of how to install Aurora is available from [MrMario2011](https://www.youtube.com/watch?v=FNYVGkFJV2s) or [Modded Warfare](https://www.youtube.com/watch?v=Kqvruf8q3J0).

- The default username/password for FTP is "xboxftp" and "xboxftp". 
- You can change your settings for FTP in the Plugins section of the menu.

## Installation

You can install it just like an App and then adjust your default in DashLaunch to point to Aurora's xex file.

You will need: 

- A console capable of running unsigned code
- [A copy of the latest Aurora build(currently 0.7b.1)](http://phoenix.xboxunity.net)
- [XexMenu]({{ site.baseurl }}/docs/consoles/microsoft/xbox360/info/software/homebrew/app/xexmenu)
- [DashLaunch]({{ site.baseurl }}/docs/consoles/microsoft/xbox360/info/software/homebrew/app/dashlaunch)
- A method of transferring files from your PC to Xbox 360(FTP, USB, SATA, etc.)

## Controls

- **A**: Enter / Confirm / Launch
- **B**: View Settings / Back
- **X**: Browse/Search games / Select multiple files or folders in file manager
- **Y**: Game details / Sync windows' working directories in file manager
- **Start**: Settings
- **Back**: System info / tools
- **LB/RB**: Change content category
- **LT/RT**: Scroll through content (fast)
- **Left Thumbstick**: Scroll through content (slow)
- **Right Thumbstick**: Peek left/right
- **DPAD**: Move left/right

## Game Launcher (CoverFlow)

The game launcher is a horizontal coverflow launcher that lists your games, apps, and other executables in a fluid and dynamic style. Aurora detects executables from user-defined paths that Aurora will load xex files from. Aurora then assigns metadata to the detected xex files using Internet access to download covers, Title Updates, descriptions, and more!

## View Settings (B)

### Filters & Sort

- Filter Content in the game launcher by type or favorites
- Set how titles are sorted
- Clear All to reset all filters

### Quick View

- Create custom filters to sort and change view.
- Disable categories

### Theme

This section allows you to modify the current theme's settings. By default, you can change the colors and speed of the aurora in the background by selecting "Override Defaults" and "Configure". You can also change the background image by placing a JPG/PNG/DDS into .../Aurora/User/Backgrounds and pressing X to refresh. The Cover Layout allows you to choose how the game covers are displayed and animated in the game launcher.

- Modify theme settings
- Default Aurora background allows changing speed and colors of the background by selecting "Override Defaults" and "Configure". 
- Add backgrounds by adding JPG/DDS/PNG files to the `Aurora/User/Backrounds` directory and pressing X to refresh options.

### Skin

A skin is a bundle that includes backgrounds, animations, cover layouts, and more for Aurora theming.

- Change active skin

### Display

- Overscan
- Toggle letterbox
- Toggle Profile Picture/Avatar
- RSS feed settings

## Browse (X)

- View your titles in a text list
- Mark games as favorites
- Search titles

## Details (Y)

- Shows details about a game/app
- Shows ratings from Xbox Live marketplace
- Shows when game/app was last launched
- Menu is comprised of options on left hand side, with additional options selectable using the left and right on the D-PAD while hovering over the various options.

## Alternate Options

- **Favorite**: Marks the game as a favorite.

- Launch

  : Launch the game.

  - **Trainer**: Allows you to select a trainer before launching the game.
  - **Settings**: After enabling Settings Override, you can set patches for the game, as well as "activator" and "trigger" buttons which act as a button combo to take in-game screenshots. 

- Title Updates

  : Allows you to view installed game updates and download more from the Unity Marketplace.

  - **DLC**: Shows installed DLC.
  - **File Manager**: Opens the file manager to the game's directory.

- Achievements

  : Shows the game's achievements

  - **Saved Games**: Lists all of your game saves.

- Preview

  : Shows game preview images (if it has any).

  - **Screen Captures**: Shows any screenshots you took.
  - **Refresh**: Redownloads all metadata for your game. This will override the game cover.
  - **Download Cover**: Shows a list of community uploaded game covers to apply.

- Rename

  : Renames the displayed name in the game launcher.

  - **Hide**: Hides the game from the main screen. Useful for hiding backups of games if you plan on modding.
  - **Delete**: Deletes the game and everything in the game directory.

## System (Back)

This section shows various tools and metadata about your temperatures and IP address. 

- **File Manager**: Opens the file manager.
- **Scripts**: Allows you to run Lua scripts which you've placed in `Aurora/User/Scripts/Utility`. 
- **Restart**: Restarts Aurora.
- **Reboot**: Power cycles your console.
- **Shutdown**: Shuts down your console. 

## Settings (Start)

### Assets

This section allows you to download metadata from the Xbox Live marketplace for all games, even from different regions. The Download button will download them from the selected locale, while the Import button will import metadata that you place on your local hard drive in the asset import format.

### Asset Import Format

**Metadata**:

> Aurora\User\Import<TitleID>\titlename.txt
>
> Aurora\User\Import<TitleID>\description.txt
>
> Aurora\User\Import<TitleID>\publisher.txt
>
> Aurora\User\Import<TitleID>\developer.txt
>
> Aurora\User\Import<TitleID>\releasedate.txt
>
> Aurora\User\Import<TitleID>\genre.txt 

**Banner**:

> Aurora\User\Import<TitleID>\banner.jpg/png/dds

**Cover**:

> Aurora\User\Import<TitleID>\cover.jpg/png/dds

**Background**:

> Aurora\User\Import<TitleID>\background.jpg/png/dds

**Screenshots**:

> (number up to 20)
>
> Aurora\User\Import<TitleID>\screenshot1.jpg/png/dds
>
> OR
>
> (number up to 20)
>
> Aurora\User\Import<TitleID>\screenshot01.jpg/png/dds

### Profile

- Set auto sign-in profile
- Add username and API Key to access XboxUnity services
  - You can get a API key by registering with XboxUnity and logging in with your username and password using the Request button.

### Content

#### Title Updates

- Allows you to control automatic scanning for updates.
- Allows you to mass install/delete title updates.
  - Requires a XboxUnity account to download updates from XboxUnity servers.

#### Manage Paths

- Add folders to be scanned for games/apps.
- Set content types for paths.
- Set search depth for paths.

#### Modules

This section shows plugins and their options. 

#### Language

This section allows you to change Aurora's language. You can add more languages by placing the language files in `Aurora/Media/Locales`.

#### Security

- Allows password protecting areas of Aurora.
- Passcode is set after applying.
- Passcode is removed if all options are unticked and applied.

#### About

- Credits
- Update Aurora
- Version Information

## File Manager

- Dual window
- Switch tab with LB/RB
- The icons on the left choose standard file management options as indicated next to the A button icon at the bottom. To exit, browse back to the root and press B.
- Uses a commander-style interface

## Troubleshooting

- **No Synopsis / Marketplace Rating**
  - Likely your router firewall is blocking the Xbox Live ports for pulling this data. You must forward the ports on your router.
- **Can't play local system link** 
  - You must unload the FreeStyle plugin any time you wish to play local system link.

If you encounter an issue not listed, please open an issue on the wiki for us to try to help solve and add!

# References

- https://www.reddit.com/r/360hacks/wiki/aurora - Thanks to the 360hacks wiki team for their work.
- Thanks to MrMario2011 and Modded Warfare for their videos on installing Aurora.