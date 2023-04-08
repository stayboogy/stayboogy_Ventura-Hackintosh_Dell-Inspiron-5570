# stayboogy Ventura Hackintosh Dell Inspiron 5570

## Working:

audio

video graphics

display backlight

hdmi output

keyboard backlight

keyboard media keys

keyboard audio keys

icloud (requires smbios editing)

wifi + bluetooth + continuity (requires proper wifi card - amazon)

airdrop

sidecar

unlock with Apple Watch

file vault

## Not Working:

keyboard display brightness keys F11/F12 (use FN+S / FN+B instead)


## Ventura Installer Image for Dell Inspiron 5570 and 5000 series Laptops

https://www.mediafire.com/file/hw2n6ttctgxim1y/stayboogy_Ventura.raw/file

1) Write the image to a flash drive of 16GB or more using your preferred method

2) if you don't know how to write this image to a flash drive, stop here, go no further


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

1) Final EFI for File Vault Compatibility with Updated Drivers and Kexts resides in a zip file on the Installer Image EFI Partition -- It is also in this repo.

2) Supplied SMBIOS Information in the Installer EFI config.plist is for installing only.  DO NOT sign into iCloud without inputing your own SMBIOS info in the Platform Section.

3) OpenCore Configurator is included in this repo so you can mount your EFI for Post Setup Tasks and so you can edit your config.plist
