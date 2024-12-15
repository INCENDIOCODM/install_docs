### Pre-installation:

* Ensure you are running the latest available stock ROM
* Optional gapps ([my Nikgapps variants](https://nikgapps.com/306bobby-android) optimized for Pixels or [official NikGapps variants](https://nikgapps.com/downloads))
* Recovery (from download page, recovery button)
* Google platform-tools (adb/fastboot)


### First time installation (clean flash):

* Step 1: Unlock bootloader and enable adb through developer settings
* Step 2: On PC enter

```
adb reboot bootloader
```
* Step 3: Now type the following command to unlock the bootloader (if necessary) and flash required images:

```
fastboot flashing unlock # If required
fastboot flash boot /path/to/boot.img
fastboot flash dtbo /path/to/dtbo.img
fastboot flash vendor_boot /path/to/vendor_boot.img
```
* Step 4: Using volume and power buttons, select "Reboot Recovery"
* Step 5: Wipe data. select Apply Update, then ADB sideload and type

```
adb sideload /path/to/ROM.zip
```
* Step 6: Reboot recovery and sideload any extras, then reboot device!

### Update installation:
* Step 1: boot phone into normal Android mode
* Step 2: Download update to phone or adb push from PC
* Step 3: Open Settings>System>Updater
* Step 4: Click the hamburger icon on the top right, then Local Update, and apply
* Step 5: Stay on this page until reboot prompt OR if the update screen goes blank, reboot / switch slots in root app
