# stayboogy Ventura Hackintosh Dell Inspiron 5570

## Working:

audio

AirPod Audio DRM Apple Music

video graphics

display backlight

keyboard backlight

keyboard media keys

keyboard audio keys

icloud (requires smbios editing)

wifi + bluetooth + continuity (requires proper wifi card - amazon)

AirDrop

sidecar iPad

unlock with Apple Watch

continuity camera

hdmi output

file vault

## Not Working:

keyboard display brightness keys F11/F12 (use FN+S / FN+B instead)


## Ventura Installer Image for Dell Inspiron 5570 and 5000 series Laptops

https://www.mediafire.com/file/hw2n6ttctgxim1y/stayboogy_Ventura.raw/file

1) Write the image to a flash drive of 16GB or more using your preferred method

2) if you don't know how to write this image to a flash drive, stop here, go no further

## Post Setup EFI

https://github.com/stayboogy/stayboogy_Ventura-Hackintosh_Dell-Inspiron-5570/blob/main/Post%20Setup/EFI-PostInstall-Rev03.zip

## Full Video Tutorial

https://youtu.be/IXkITt6ZECU


## Simplified Directions

1) Write the Installer Image to Flash Drive
2) Set BIOS Settings for MacOS
3) Boot from Installer Flash Drive
4) Install MacOS
5) Copy EFI from Installer Flash Drive to EFI Partition on HDD

Optional:

6) Do your own SMBIOS Editing for iCloud if needed (do not use supplied SMBIOS Info)
7) Turn on FileVault
8) Sign into iCloud
9) Enjoy MacOS in all its Glory
10) follow stayboogy

## Notes

1) This process assumes you are using two disks like I am here.  If you are installing MacOS on the same disk as Windows, A) Backup your EFI folder structure to another usb first before starting this process, B) Delete "Clover" and/or "OC" folder that may be present in that EFI backup, C) Make sure the "Microsoft" folder and "Boot" folder remain, D) After this entire process is completed as shown here in the video, copy this backup into the EFI folder on the hard drive that we just copied from our usb installer.

2) Supplied SMBIOS Information in the Installer EFI config.plist is for installing only.  DO NOT sign into iCloud without inputing your own SMBIOS info in the Platform Section.

3) OpenCore Configurator is included in this repo so you can mount your EFI for Post Setup Tasks and so you can edit your config.plist.

4) All Continuity Features are working, but they require a compatible wireless network card - I got mine off Amazon and I have all everything working.

5) For AirPod Audio Streaming to working from Apple Music and Apple TV, you must authorize your computer from the Account menu in each app.

6) Final EFI to be installed to HDD after install is completed is in this repo - use the latest revision instead of the EFI on your installer flash drive.
