# PostSetup

## PostSetup_EFI_Rev08.zip

1) unzip
2) run MountEFI
3) delete all files on hdd EFI partition that was mounted
4) copy over unzipped EFI folder to recently mounted hdd EFI partition
5) reboot

## MountEFI
    script executable I made that Mounts the EFI Partition of the HDD
    
	Right Click and Open in Terminal
	or
	Double Click to run

## DisplaySleepLock 
    script executable I made to Lock and Sleep the Display 
    before closing lid to overcome not asking for password 
    when lid is closed and then reopened before 
    "pmset displaysleeptime value" in pmsetter

## pmsetter 
    script executable I made to set the proper Power Settings for the only sleep that works
    
	Right Click and Open in Terminal
	or
	Double Click to run

	*This is the best possible setting for 
        having nice battery but being able to wake up 
        after closing the lid or the display goes to sleep on its own
	
	1) Sets no "deep" sleep and no "hibernation" and the display to turn off after 2 minutes.
    
	2) You can change this by opening in TextMate (PostSetupApps.zip) 
        and changing all instances of "displaysleep 2" to whatever number 
        you want in minutes for the display to cut off.
    
	3) If you close the lid, it will not ask for password when opening 
        unless the same 2 minutes, or the number you choose 
        to put there if you edit pmsetter, passes and then is not guaranteed.
    
		A) so use the included "DisplaySleepLock" executable 
            to lock your machine before closing the lid 
        
            or 
        
		B) you can lock from the Apple Menu before closing the lid 
            so that password is required when you open the lid 
            if done before your displaysleep time setting

## neofetch 
    executable to see your Mac Info nice and neat like in my screenshot

## PostSetupApps.zip

1) GenSMBIOS - generate SMBIOS information for your hackintosh
	Choose ONLY:
	MacBook10,1 (low end dual core configuration) 
	MacBookPro14,1 (appropriate cpu and graphics profile) 
	MacBookPro14,2 (appropriate cpu and graphics profile--high end) 
	MacBookPro15,2 (best cpu and graphics profile--what I use)

2) MaciASL - DSDT and SSDT software

3) LockSleep - App I made to do what DisplaySleepLock does above - useful to put into dock to make it an easy process

4) OpenCore Configurator.app - For editing your config.plist

5) TextMate.app - better text editing app - edit anything including config.plist

6) ProperTree_Ventura.zip - config.plist editor
	A) Install the Python Package first or else ProperTree will not run
	B) Ventura specific build I made from source


