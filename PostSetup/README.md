# PostSetup Process

1) Run "MountEFI" to mount the EFI partition
2) Unzip PostSetup_EFI_Rev08.zip
4) delete all files on hdd EFI partition that was mounted
5) copy over unzipped EFI folder to recently mounted EFI partition
6) reboot
7) reset nvram
8) Run "PostPowerPerf.app" to set my custom Power Manager Settings
9) Enjoy

## PostSetup_EFI_Rev08.zip

1) unzip
2) run My MountEFI
3) delete all files on hdd EFI partition that was mounted
4) copy over unzipped EFI folder to recently mounted hdd EFI partition
5) reboot
6) reset nvram

## MountEFI
    Executable I created to Mount EFI Partition

## PostPowerPerf.app
    App I created to configure the only working power manager settings 

## LockSleep.app 
    App I created to lock and sleep the screen.
    
    This is the only sleep and wake that works.
    
    After Running PostPowerPerf, you must click LockSleep before you close your lid.
    
    Closing the Lid will only cut off the display, it will not Lock your Screen or Account.
    
    This is due to my custom power settings, which are set due to incompatible BIOS power code.
    
    LockSleep overcomes this issue.  LockSleep will immediately lock your device and sleep the display.
    
    Apple Menu-->Lock Screen does basically the same thing other than sleeping the screen.  
    
    My app is a one-click solution.
    
## ThirdPartyApps

- GenSMBIOS - generate SMBIOS information for your hackintosh

	Choose ONLY:

	- MacBook10,1 (low end dual core configuration) 

	- MacBookPro14,1 (appropriate cpu and graphics profile--good)
 
	- MacBookPro14,2 (appropriate cpu and graphics profile--high end)
 
	- MacBookPro15,2 (best cpu and graphics profile--top tier, what I use)

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


