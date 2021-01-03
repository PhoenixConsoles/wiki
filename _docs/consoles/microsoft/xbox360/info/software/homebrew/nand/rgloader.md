https://mega.nz/#!nVVWkAab!3c5Lb50ff1xdsVAyWhoa9ZIgkHRE3tew_UNP6kwkODE



## options.ini settings

````ini
[Options]
Phat_Precompiled_CD = yes
Generate_Dummy_KV = no

;-----------------
[Patches]
;disable fcrt.bin for slims
NOFCRT = 0
;disable internal MU for big block jaspers.. even though we don't really support those
NOMU = 0
;set systemroot to hdd
SYSROOTHDD = 1
;set systemroot to usb thumb drive
SYSROOTMASS = 0
;patch kd connect retries to 1
kd_1retry = 1
;disable stock bootanim (neccesary for rgloader bootanim)
disable_bootanim = 0
;freeboot style peek poke with syscall 0
HVPEEKPOKE = 1
;disable memory protection (fixes stuff like trainers, no need for dmsetmemory)
NOMEMPROT = 1
;disable shadowbooting on system boot (speeds bootup a bit)
NOSHADOWBOOT = 1

;-----------------
[Directories]
NAND_data = ..\nanddata
loaders = ..\loaders
patches = ..\patches
release = ..\rls
bin = ..\bin
defaults = ..\builds\defaults
build = ..\builds
filesystems = ..\filesystems

[Xell]
xell_binary = xell-gggggg.bin
xell_path = ..\

[Default_INI]
fat = fat.ini
fatRGH2 = fatRGH2.ini
slim = slim.ini

[Output]
output_file_location = ..\

[RGLauncher]
CPU_Key = 988A1FC50DEBBEC0D3D919F03640F300 ;a duplicate entry for the CPU_Key, remove this.
CPU_Key = 00000000000000000000000000000000 ;this is where you enter the CPU Key for your console.
exploit = JTAG ;this is where you enter either RGH(for RGH1), RGH2, or JTAG to build the correct NAND.
kernel = 17150 ;this is where you enter the kernel version you want, found in the Filesystem folder.
nand_location = NAND ;this is where the program stores the location of the NAND image on your computer for reference.
rglversion = 0v500 ;this is the version of you

````



## rgloader.ini settings

````ini
[Filters]

Block_Live_Dns = 0  ;block xbox live servers


[Expansion]

Map_USB_Mass = 1  ;map usb drives to xbox neighborhood

Persistent_Patches = 1 ;enable patch reloading on every xeximageload.

;Boot_Animation_Path = \SystemRoot\RGL_bootanim.xex ;path to new bootanim xex
;Boot_Animation_Movie = Hdd:\bootanim.wmv ;path to new bootanim xex

HUD_Jump_To_XShell = 1 ;Replaces family settings button in HUD with "Return to XShell"

Retail_Profile_Encryption = 0 ; Enables retail profiles on devkit kernel
;*WARNING: This may corrupt live profiles! Do not enable this patch if you have profiles you want to keep clean!


[Config]

;Default_Dashboard = \SystemRoot\dash.xex  ;sets the metro dash as the default dash

Default_Dashboard = \Device\Flash\xshell.xex  ;sets the devkit launcher as the default dash

;Redirect_Xshell_Start_But = \Device\Harddisk0\Partition1\FSD\default.xex  ;redirect start button in xshell

No_Sign_Notice = 0  ;Disables xbox live signin warning when enabled

Use_RGLP_Patches = 1 ;apply runtime patches to xam 

[Plugins]
Plugin1 = none
Plugin2 = none
Plugin3 = none
Plugin4 = none
Plugin5 = none
````

## 