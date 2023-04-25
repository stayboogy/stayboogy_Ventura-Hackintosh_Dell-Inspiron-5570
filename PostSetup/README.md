# PostSetup Process

1) Run "MountEFI" to mount the EFI partition

or

1) Run OpenCore Configurator-->Tools-->Mount EFI
2) Unzip stayboogyVentura-PostSetup-EFI-Rev13.zip 

or 

2) Unzip stayboogyVentura-PostSetup-EFI-Rev13-WiFi.zip
4) delete all files on hdd EFI partition that was mounted
5) copy over unzipped EFI folder to recently mounted EFI partition
6) reboot
7) reset nvram - See Below
8) Enjoy

## stayboogyVentura-PostSetup-EFI-Rev13.zip / stayboogyVentura-PostSetup-EFI-Rev13-WiFi.zip

1) unzip
2) run My MountEFI
or
2) Run OpenCore Configurator-->Tools-->Mount EFI
3) delete all files on hdd EFI partition that was mounted
4) copy over unzipped EFI folder to recently mounted hdd EFI partition
5) reboot
6) reset nvram
7) open terminal and run:
    "sudo pmset -a restoredefaults"
    
## Reset NVRAM from OpenCore Boot Menu

- After any changes to your config.plist
- After any SMBIOS changes
- After any update to the System EFI

## MountEFI
    Executable I created to Mount EFI Partition
    
## ThirdPartyApps

- GenSMBIOS - generate SMBIOS information for your hackintosh
    - DO NOT sign into iCloud without inputing your own SMBIOS info in the Platform Section.
    - MacBookPro14,2 is the Only SMBIOS platform to use - 
    - Make sure you never use a real valid key - test every configuration
    - Change a few characters in every item that GenSMBIOS / OpenCore Configurator gives you
    - ALL SMBIOS Data is important for All the Real Features of using a MacBook

- MaciASL 
    - DSDT and SSDT software

- NeoFetch 
    - System Information generator like my screenshot

- OpenCore Configurator.app 
    - For editing your config.plist

- TextMate.app
    - better text editing app - edit anything including config.plist

- ProperTree_Ventura.zip - config.plist editor
	- Install the Python Package first or else ProperTree will not run
	- Ventura specific build I made from source


