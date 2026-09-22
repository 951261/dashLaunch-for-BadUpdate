# Dashlaunch GUI for BadUpdate/ABadAvatar
This is a WIP attempt to modify dashlaunch to work on Xbox 360s running BadUpdate and ABadAvatar. This allows you to edit you launch.ini settings (such as pluggins) with the polished Dashlaunch user interface. 

### Modifications I made:
* Removed all NAND modifying code (apart from FTP) to prevent bricking the console
* Prevent the installation prompt from being displayed on startup
* Dissabled the `Install`, `Uninstall`, `Update Patches`, and `Install This` buttons

### Known Issues
* launch.xex should be loaded before launching this program. XeUnshacked should handle this automatically.
* launch.xex cannot be loaded by this program. If you select the unload option, do not expect to be able to select load without crashing your console
* It is still possible to modify the flash over FTP! When accessing the console over FTP, no matter what FTP server you are using (Dashlaunch, Aurora, etc...) you should NEVER modify your main flash memory, as it will probably brick your console. 

### TODO
* Prompt to save settings upon attempting to exit - I cannot count how many times I have changed a dashlaunch setting, only to press B and have none of my changes saved.
* Get fan controls working
* Double check the code to ensure there are no NAND writes I have missed. 

### Credits

* Many thanks to cOz for their incredible work creating DashLaunch
* Many thanks to everyone else, and their open source projects that made dashlaunch possible. cOz created a list of thankyous in [/ReadMe/readme.txt](/ReadMe/readme.txt)
