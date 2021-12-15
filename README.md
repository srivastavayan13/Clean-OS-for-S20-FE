# Clean-OS-for-S20-FE
this script can be used for atleast any dynamic partition samsung device
This zip contains all the codes required to flash your modified files into the system
Put your system.img in place of the system.img file in there
Put your boot.img with custom kernel installed and magisk if you want too ( You can pull the boot.img from your devie by using termux)
Code for pulling boot.img from your device is 1. su 2. grant permission 3. dd if=/dev/block/by-name/boot of=/sdcard/boot.img 4. copy the file from internal storage
you can use modified up_param.tar for removing bootloader warning for your device
Now coming to the clean folder it contains 
1. Mods - in here dont touch the system folder instead open it and place whatever mods you decide to add in your system folder
2. vendor - in here you can put whatever changes you want to do in your vendor folder. For example i have put dummy floating feature 
3. Restore - you can use to restore or install any app you want. Create a new folder with your app name under which create a folder named system then create at which path in system you want to add those app like either in app or priv-app and then create a folder with your app name again and under which put the apk file
4. Meta-Info folder has addons folder which you can use to flash external zip you want to flash with your build, in my case i have put multidisabler to be flashed with my build. Check updater-script for the same 
5. Update Updater-script as per your requirement. I have given many option and for installing apps i have given option to either install or dont install them, leaving choice for the end-user whether they want a particular app or not
