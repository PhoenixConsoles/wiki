# Setting up a Xbox 360 Development Environment on Windows 10

Disclaimer: This is purely for educational purposes. What you do with this information is your responsibility.

## Microsoft Official SDK

### You will need to install:

You can install the following manually or install it all via the [Visual Studio 2010 Ultimate setup](https://visualstudio.microsoft.com/vs/older-downloads/).

If using the websetup: 

1. Deselect the option to send information about setup to Microsoft.
2. Accept the license terms and continue.
3. Choose a full install. It will take approximately 7 GB.

If installing manually: Install...

````
.NET Framework 4

Microsoft Application Error Reporting

VC 9.0 Runtime

VC 10.0 Runtime

Microsoft Visual Studio 2010 Prerequisites

Microsoft Visual F# 2.0 Runtime

Microsoft Visual Studio Macro Tools

TFS Object Model

.NET Framework 4 Multi-Targeting Pack

Microsoft Visual Studio 2010 Ultimate

Microsoft Web Deployment Tool

Microsoft ASP.NET MVC 2 - Visual Studio 2010 Tools

Microsoft ASP.NET MVC 2

Microsoft Silverlight

Microsoft Silverlight 3 SDK

Microsoft Visual Studio 2010 Tools for Office Runtime

Microsoft Office Developer Tools

Dotfuscator Software Services - Community Edition

Crystal Reports templates for Visual Studio 2010

Microsoft SQL Server Compact 3.5 SP2 ENU

Visual Studio 2010 Tools for SQL Server Compact 3.5 SP2 ENU

Microsoft Sync Framework Runtime v1.0 ENU

Microsoft Sync Services for ADO.NET v2.0 ENU

Microsoft Sync Framework Services v1.0 ENU

Microsoft Sync Framework SDK v1.0 ENU

VC 10.0 Designtime

Microsoft Visual Studio 2010 Performance Collection Tools

Microsoft Visual Studio 2010 IntelliTrace

Microsoft SQL Publishing Wizard 1.4

Microsoft SQL Server System CLR Types

Microsoft SQL Server 2008 R2 Management Objects

Microsoft SQL Server 2008 Express Service Pack 1

Microsoft SQL Server 2008 R2 Data Tier Application Framework

Microsoft SQL Server 2008 R2 Data Tier Application Project

Microsoft SQL Server 2008 T2 Transact-SQL Language Service

Microsoft SharePoint Developer Tools

Microsoft Visual Studio 2010 ADO.NET Entity Framework Tools

Microsoft Help Viewer 1.0
````

Now Visual Studio 2010 Ultimate is installed and activated with a trial key. You can get a full version key [here](https://www.google.com/search?q=visual+studio+2010+key). 

Now, you must:

1. Run Visual Studio 2010 to set it up and activate it with a full license key that you have purchased from Microsoft.
2. Install the [Visual Studio 2010 SDK](https://www.microsoft.com/en-us/download/details.aspx?id=21835), [MSXML 6.0 package](https://www.microsoft.com/en-us/download/details.aspx?id=3988), and [MSXML 4.0 SP2 Parser and SDK](https://www.microsoft.com/en-us/download/details.aspx?id=19662) for additional functionality and documentation.
3. Install the Xbox 360 SDK and choose Full Installation.

You now have a fully working Xbox 360 Development Environment on Windows 10! You can now create, compile, debug, and package software for the Xbox 360!

## Open360SDK

Open360SDK is a under-development tool by Phoenix Consoles' OpenXenon project to have all the functionality of the official Microsoft Xbox 360 SDK but built from the ground up and completely open source. To learn more, check out the website.