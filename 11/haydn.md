### Pre-installation:

* Gapps: [NikGapps](https://nikgapps.com/downloads) or [CrGapps](https://nikgapps.com/crdroid-official)
* Optional: [KernelSU](https://github.com/tiann/KernelSU)
* TWRP and Boot: [Download](https://sourceforge.net/projects/crdroid/files/haydn/11.x/boot/) (Download any one Depending how you want to install)

### Installing TWRP

* You need to have [Platform Tools](https://developer.android.com/tools/releases/platform-tools) in your PC (Navigate to ***"Download SDK Platform-Tools for Windows"***)
* Now go to Downloads and Unzip it. 
* Open the folder and search 
```
cmd
```
* It will open the Terminal
* Now on the phone hold the ***POWER + VOLUME Down*** together for 5-10 seconds until the phone enters the Fastboot Mode
* Now type
```
fasboot devices
```
* Your device will be shown in the terminal as a Fastboot Device
* Now type
```
fastboot boot drag-and-drop-the-twrp-image
```
* Now you are booted to TWRP

### Fisrt Time Installation

* ### installing  via TWRP
* ***Note: Please go through the Installing TWRP once***
* Backup your data to PC, OTG flash drive.
* Open the Platform Tools in PC
* Type
```
cmd
```
* Hold the Power and Volume Up buttons together for 5-10 seconds until it boot to TWRP
* Now Navigate to ***WIPE > ADVANCE WIPE***
* Select: ***data, metadata, cache, Dalvik Cache***
* After wiping go back and navigate to ***Install***
* Select the Crdroid Zip and the Gapps (if any)
* After the flash is done, Simply Reboot
* Enjoy !!!



### Installing Via Cr Recovery
* Firtly, boot to fastboot
* On pc terminal type 
```
fastboot boot drag-and-drop-the-image
```
* Now in recovery go to factory reset and confirm the reset
* Reboot to recovery
* Choose apply update and Apply from ADB
* Now install crDroid zip via sideload with
```
adb sideload drag-and-drop-the-zip
```
* Reboot To Recovery
* Flash Gapps with
```
adb sideload drag-and-drop-the-gapps
```
* Reboot and Enjoy !!!

### Update installation:

### 1. Using TWRP
* Boot to TWRP Recovery (Hold Pow + Vol Up)
* Download the the update zip in the storage of the device
* Choose Install 
* Select the crDroid.zip and Gapps (if the phone has Gapps before update)
* Reboot and Enjoy !!!

### 2. Using Cr Recovery
* Boot to Cr recovery (Hold Pow + Vol Up)
* Open Terminal in your pc (in the the Platform tools folder)
* Type:
```
adb devices
```
* It will show your and device code and mode type
* Now head to the recovery: ***Apply Update > Update Via ADB***
* Now type: (in Terminal)
```
adb sideload drag-and-drop-cr.zip
```
* Flash Gapps
```
adb sideload drag-and-drop-gapps.zip
```
* Reboot and Enjoy !!!

### 3. Update Via OTA
* Go to Settings -> System -> Updater and download latest build
* Choose install and let it finish
* If having gapps, reboot to recovery and sideload gapps package again
* Reboot
