# Converting a Game on Demand (GOD) to an ISO

#### See More

1. Game on Demand

2. XISO

3. ISO


### Scope

This guide will walk you through the conversion of a GOD container to an ISO. 

### Goals

- To convert a GOD container to a ISO

### Prerequisites

- Windows PC
- Xbox 360 capable of running unsigned code
- A GOD container
- [GOD2ISO](http://www.mediafire.com/download.php?o7sf7f8687p7tux)

## Converting GOD to ISO

**Verify that your GOD container is complete.**

### Converting with GOD2ISO

When you open GOD2ISO you will be greeted by this window:

![A screenshot of the GOD2ISO v1.0.4 main window]({{ site.baseurl }}/_media/software/god2iso/main.jpg)

1. Click `Add...` to add GOD files to convert to ISO. You will be greeted with a file explorer to explore to the GOD identification file.  Select `Open` and repeat for as many GOD containers as you wish.

2. Click `Browse...` to select an output path for the ISO file(s). You will be greeted with a file explorer to explore to a directory that will be the output directory for the resulting ISO(s) for each GOD container selected.

3. Check the box next to `Fix "CreateIsoGood" broken header`, otherwise the XISO header will be invalid and extraction programs and the Xbox 360 will not recognize the resulting ISO.

4. Click `Go!` to begin the conversion process. The resulting file for each ISO will be stored in the selected output directory as once it is completed. When it is complete there is no notification, but you will know the process is complete when the buttons are no longer greyed out and the progress bar is moved all the way to the right for both `Iso progress:` and `Total progress:` as shown in the following screenshot: 

   ![A screenshot of the GOD2ISO v1.0.4 main window after the completion of conversion, indicated by the progress bars being all the way to the right and the Add, Clear, Browse, and Go buttons being no longer greyed out.]({{ site.baseurl }}/_media/software/god2iso/finished.jpg)

## Help

Need help? Having an issue? Want to suggest an addition or change? [Submit an issue!](site.repo)

### Troubleshooting

Troubleshooting information for GOD2ISO can be found [here.]( {{site.baseurl}}/_docs/consoles/microsoft/xbox360/info/software/homebrew/fsft/god/god2iso.html#troubleshooting)

# References

- [Converting a Game on Demand (GOD) to ISO on r/360hacks wiki](https://web.archive.org/web/*/https://www.reddit.com/r/360hacks/wiki/god2iso) [[Direct Link]](https://www.reddit.com/r/360hacks/wiki/god2iso)