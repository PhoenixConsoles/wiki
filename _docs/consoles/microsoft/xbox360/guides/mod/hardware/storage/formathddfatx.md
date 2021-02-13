---
title: Formatting an accessory storage device for the Xbox 360 as FATX
description: Short paragraph describing the page.
tags:
 - guides
 - xbox 360
 - microsoft
 - consoles
 - fatx
---

# Formatting an accessory storage device for the Xbox 360 as FATX

### Disclaimer

**This is solely for educational purposes. You are responsible for your usage of this information and for any damage, or anything else that may occur as a result of accessing this educational material. Please ensure you are complying with applicable laws for your region. Accessing this page is acceptance of this disclaimer.**

### Scope

This guide will show you how to format an accessory storage device for the Xbox 360 as FATX.

### Goals

- Format the accessory storage device as FATX on an Xbox 360
- Format the accessory storage device as FATX on a Windows PC
- (TBD) Format the accessory storage device as FATX on Linux
- (TBD) Format the accessory storage device as FATX on Mac OS

### Prerequisites

- Xbox 360 console and controller (if using Xbox 360 to format HDD)
- Xbox 360 accessory storage device or off-the-shelf storage device (Freeboot and XDK only)
- A Windows PC and FatXplorer (If using a Windows PC)

### Warnings and Notices

- Once the HDD is formatted, if the HDD is not an official Microsoft HDD then the compatibility partition will need to be repaired.

## Formatting the accessory storage

### From the Microsoft official dashboard

#### Blades

From the Blades dashboard, navigate to the `System` blade and select `Memory`. Select your storage device to format and press **Y**. Select `Format` and select `Yes` at the prompt confirming whether you would like to format the accessory storage. You will be prompted to `Enter Serial Number` at which point you will select the option and enter your console's serial number to format the accessory storage device.

#### New Xbox Experience

From the New Xbox Experience dashboard, select the `System Settings` tile of the `My Xbox` row. Select the `Memory` option and select your storage device and press **Y**. Select `Format` and select `Yes` at the prompt confirming whether you would like to format the accessory storage. You will be prompted to `Enter Serial Number` at which point you will select the option and enter the console's serial number to format the accessory storage device.

#### Kinect Update 

TBD

#### Metro

From the `home` tab, navigate to the `settings` tab using 
**LB**/**RB**, the **D-PAD**, or **left thumbstick**. Navigate to the `System` tile and select it with the **A** button. Navigate to the `Console settings` selection and press **A**. Scroll down to `System Info` and press **A**. Note down the contents of the `Console Serial Number` field. Navigate to the `Storage` selection and press **A**. Navigate to the option indicating the accessory HDD with this icon: TBD. Open `Device Options` by pressing the **Y** button with it selected. Select the `Format` option and select it with the **A** button. Confirm you wish to format and erase the contents of the selected storage device by navigating to and selecting `Yes`. Select the `Enter Serial Number` option and enter the serial number we noted down earlier. You will see a `Formatting in progress` screen and will need to wait for the formatting process to complete.  [LINK NEEDED]

### From a Windows PC

#### Using FatXplorer

From FatXplorer, select `Formatting Tools` from the toolbar. Select the type of device you wish to format (in this case a Xbox 360 HDD). You will be greeted with the Xbox 360 HDD formatting wizard. Select `Next` and move to the Device Select screen, where you will select the physical drive that represents the accessory storage you intend to format. Select `Next` and move on to the Configure Partitions screen, where you can select which partitions to format and set Allocation Unit/Cluster Size. Select `Next` and move on to the Security Sector step. You can restore a security sector that matches the accessory storages serial number, firmware revision, and model information. If you are using the HDD with a XDK or FreeBoot console you do not need a security sector added to the accessory storage. If you wish to restore an HDDSS.bin, select `Add S. Sector.` and browse to and select your HDDSS.bin you wish to restore. Once the security sector is restored you will be greeted with a message reading `Security Sector added.` and information about the security sector. If the accessory storage already has a security sector, the information will be displayed there from the start and there is no need to restore a HDDSS.bin, though backing it up would be wise. Select `Next` to move on to the name selection screen where you can type a name to be added to your newly formatted Xbox 360 accessory storage. Select `Next` to move to the Review screen to confirm your selected settings. Select `Next` to begin formatting. Once you are greeted with the `Formatting completed successfully` screen you can select `OK` to complete the process. You will be greeted by the Done screen of the wizard and may select `Finish` to close the wizard.

## Help

Need help? Having an issue? [Submit an issue!]( {{site.baseurl}}/pages/issues/)

### Troubleshooting

This is where you put troubleshooting information for people following this guide or link to the troubleshooting section(s) of the appropriate page(s).

# References

This is where all reference material goes, organized in bullet points like so:

- [FatXplorer Program](https://web.archive.org/web/*/https://fatxplorer.eaton-works.com/) [[Direct Link]](https://fatxplorer.eaton-works.com/)
- Independent Research (This reference indicates this page relies partially or completely on independent research. Citations are needed.)

### See more

1. Transferring data to/from the Xbox 360