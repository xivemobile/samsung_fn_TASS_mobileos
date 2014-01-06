Samsung FN TASS MobileOS
====================================

Compile using kitchen:

1. Create a folder named "xmos" in kitchens "original_update" directory, then "cd PATH_TO_KITCHEN/kitchen/original-update/xmos"

    git clone git://github.com/xivemobile/samsung_fn_TASS_mobileos.git


2. After cloning the repo open the kitchen

    ./menu


3. Set up the working folder

    1 - Set up working folder from ROM
    
    Enter option: 1 <ENTER>


  * On the next page press <ENTER> again to continue
  * You will now see a list of "Available ROMs:"

        Available ROMs:
        
          (1) xmos


         Enter selection number (default=1, cancel=0, r=refresh): 1 <ENTER>

__Chose the number from xmos (If you do not have any roms in the original-update folder, xmos will be at pos 1)__


	* Now chose a name for the working folder (Press enter or n to use the default one)

    The new working folder will be named WORKING_010614_234820 (for example)
	Change the name (y/n)? (default: n): n <ENTER>


After the ROM has been copied to the working dir you have to choose wether to convert the update script to the "Amend format" advanced compatibility for further settings or the "Edify format" to keep the original updater-script.

	1 = Convert it to update-script (Amend format)
    2 = Do nothing, keep updater-script (Edify format)

    Choose 2 <ENTER>


After that yu'll see a small list of files containing in woring folder

    Press Enter to continue


Now you wish to compile and sign the ROM

    99 - Build ROM from working folder

    Enter option: 99

    after that select "build option" 1 (Interactive Mode - recommended for most users) <ENTER>

    If you were asked "Would you like to optimize the APK files by zipaligning them (y/n)? (default: y):" press y and <ENTER>

    After Making update.zip you'll be asked for "It is recommended that you sign your ROM. Sign it (y/n)?" press y and <ENTER>


It may take some time... when it is ready you'll see a message like:

    The new ROM will be named tass_signed_010614_235715.zip (for example)
	Change the name (y/n)? (default: n):

select `n` and press `<ENTER>`

your rom is located in the "OUTPUT_ZIP" directory



@res    [Android Kitchen 0.224 - by dsixda (xda-developers.com)](https://github.com/xivemobile/Android-Kitchen)