# stayboogy Ventura Hackintosh Dell Inspiron 5570

MacOS Ventura Hackintosh Dell Inspiron 5570 (stayboogy)

![App Screenshot](https://github.com/stayboogy/stayboogy_Ventura-Hackintosh_Dell-Inspiron-5570/blob/main/neofetch_SystemInfo.png)

## Working:

https://youtu.be/VAYKbTMqm4k

Working:

Trackpad
SDCard Reader
Audio
AirPod Audio DRM Apple Music
Video Graphics
Display Backlight
Keyboard Backlight
Keyboard Media Keys
Keyboard Volume Keys
iCloud + iMessage + FindMy + ETC (requires smbios editing)
WiFi + Bluetooth + Continuity (requires proper wifi card - amazon)
AirDrop
Sidecar iPad
Unlock with Apple Watch
Continuity Camera
HDMI Output
File Vault

Not Working:

Keyboard Brightness Keys (can be set in Keyboard Shortcuts Settings)

## Not Working:

keyboard display brightness keys F11/F12 (use FN+S / FN+B instead)


## Ventura Installer Image for Dell Inspiron 5570 and 5000 series Laptops

https://www.mediafire.com/file/miuye8v898qh7gw/stayboogy_VenturaUSB.raw/file

MD5: daef5af0cad299d5d7787fc0e456336e

1) Write the image to a flash drive of 16GB or more using your preferred method

2) if you don't know how to write this image to a flash drive, stop here, go no further

## Post Setup EFI

https://github.com/stayboogy/stayboogy_Ventura-Hackintosh_Dell-Inspiron-5570/blob/main/Post%20Setup/PostSetup_EFI_Rev08.zip

## Full Video Tutorial

https://youtu.be/VAYKbTMqm4k


## Simplified Directions

1) Write the Installer Image to Flash Drive
2) Set BIOS Settings for MacOS
3) Boot from Installer Flash Drive
4) Install MacOS
5) Copy PostSetup EFI to EFI Partition on HDD

Optional:

6) Do your own SMBIOS Editing for iCloud if needed (do not use supplied SMBIOS Info)
7) Turn on FileVault
8) Sign into iCloud
9) Enjoy MacOS in all its Glory
10) follow stayboogy

## Notes

1) Supplied SMBIOS Information in the Installer EFI config.plist is for installing only.  DO NOT sign into iCloud without inputing your own SMBIOS info in the Platform Section.

2) OpenCore Configurator is included in this repo so you can mount your EFI for Post Setup Tasks and so you can edit your config.plist.

3) All Continuity Features are working, but they require a compatible wireless network card - I got mine off Amazon and I have all everything working.

4) For AirPod Audio Streaming to working from Apple Music and Apple TV, you must authorize your computer from the Account menu in each app.

5) Final EFI to be installed to HDD after install is completed is in this repo - use the latest revision instead of the EFI on your installer flash drive.
