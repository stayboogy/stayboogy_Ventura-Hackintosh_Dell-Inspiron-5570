# stayboogy Ventura Hackintosh Dell Inspiron 5570

MacOS Ventura Hackintosh Dell Inspiron 5570 (stayboogy)

- My Device Specifications 
	- Dell Inspiron 5570
	- BIOS v1.13 - Must have v1.7 or higher for best results
	- i5-8250u Quad Core Kaby Lake R 
	- Integrated UHD 620 Graphics
	- BCM94360NG 802.11a/b/g/n/ac 
	- 3 USB-A Ports + SDCard Reader
	- With DVDRW or Without both devices are identical internally
	- I have 2 SSDs, 1 x 2.5" 1TB, 1 x m.2 500GB
	
## Full HD Install Tutorial Video + Feature Showcase

[[https://youtu.be/VAYKbTMqm4k]](https://youtu.be/VAYKbTMqm4k)

![App Screenshot](https://github.com/stayboogy/stayboogy_Ventura-Hackintosh_Dell-Inspiron-5570/blob/main/SysInfo.png)

## Working:

- EVERYTHING!

- Sleep + Wake + Shutdown + Restart (AC + Battery)
	- Powernap and Full Hibernation Support (Rev 13)
	- Long Wakes From Long Sleeps Just like a Real Macbook
	- Shutdown and Restart Fully Working
		- Sometimes slower and Faster based on lots of factors
		- Just like a Real Macbook
	- Notifcations While Asleep, Keep Alive, Find My Location Services, etc All Working
	- Literally Just like a Real Macbook (which I have)
	- Fully Working with Default Power Settings
		- Modify if you wish
		- I do not guarantee every possible config will work
		- I see no difference from my Real Macbook in behavior
	
- Full SMC Control ie. Macs Fan Control Fully Working
- Trackpad
- SDCard Reader
- Audio
- AirPod Audio DRM Apple Music
- Video Graphics
- Display Backlight
- Keyboard Backlight
- Keyboard Media Keys
- Keyboard Volume Keys
- iCloud + iMessage + FindMy + ETC (requires smbios editing)
- WiFi + Bluetooth + Continuity (requires proper wifi card - amazon)
- AirDrop
- Sidecar iPad
- Wireless Display
- Unlock with Apple Watch
- Continuity Camera
- HDMI Output
- File Vault

## Not Working:

- Keyboard Display Brightness keys F11/F12 (use FN+S / FN+B by default)
  - these can be changed in Keyboard Shortcut Settings back to F11 and F12

## Ventura Installer Image for Dell Inspiron 5570 and 5000 series Laptops

https://www.mediafire.com/file/w5ax5oduvkrhqo5/stayboogy_Ventura_Rev13.raw/file

MD5: d4dfe604185ce3e99310889a5b8d0191

- Write the image to a flash drive of 16GB or more using your preferred method

- If you don't know how to write this image to a flash drive, stop here, go no further

## Post Setup EFI

-Without Compatible Wifi Card / Ethernet / Non-Native Apple BT+WiFi Cards or Adapters
https://github.com/stayboogy/stayboogy_Ventura-Hackintosh_Dell-Inspiron-5570/blob/main/PostSetup/stayboogyVentura-PostSetup-EFI-Rev13.zip

-With Compatible Native Apple Wifi+BT Card
https://github.com/stayboogy/stayboogy_Ventura-Hackintosh_Dell-Inspiron-5570/blob/main/PostSetup/stayboogyVentura-PostSetup-EFI-Rev13-WiFi.zip

## Full Video Tutorial 

https://youtu.be/VAYKbTMqm4k

## Simplified Directions

1) Write the Installer Image to Flash Drive
2) Set BIOS Settings for MacOS
3) Boot from Installer Flash Drive
4) Install MacOS
5) Copy PostSetup EFI to EFI Partition on HDD
6) Reboot
7) Reset NVRAM
8) Enjoy

Optional:

9) Do your own SMBIOS Editing for iCloud if needed (do not use supplied SMBIOS Info)
10) Turn on FileVault
11) Sign into iCloud
12) Enjoy MacOS in all its Glory
13) follow stayboogy

## Notes

1) Supplied SMBIOS Information in the Installer EFI config.plist is for installing only.  
	- DO NOT sign into iCloud without inputing your own SMBIOS info in the Platform Section.
	- MacBookPro14,2 is the Only SMBIOS platform to use
	- Installer is set as MacBookPro14,1 and you SHOULD change to 14,2 whether you use iCloud or not
	- Make sure you never use a real valid key - test every configuration
	- Change a few characters in every item that GenSMBIOS / OpenCore Configurator gives you
	- ALL SMBIOS Data is important for All the Real Features of using a MacBook

2) OpenCore Configurator is included in this repo so you can mount your EFI for Post Setup Tasks and so you can edit your config.plist.

3) All Continuity Features are working but they require a compatible wireless network card.

4) For AirPod Audio Streaming to work from Apple Music and Apple TV, you must authorize your computer from the Account menu in each app.

5) The Final EFI to be installed to HDD after install is in this repo - use the latest revision instead of the EFI on your installer flash drive.
