Instructions are in each .mnu file - use Notepad to read the .mnu files.

You can place .mnu and payload files in the \_ISO\MAIMMENU folder or subfolder. You can also place it in your Sub-Menu folders.

For example, if the instructions say to place files in the \_ISO\xxxx\Utility folder:
If you place the .mnu file and .iso file in the \_ISO\MAINMENU\Utility folder, the entry will be listed in the Main Menu.
If you place the .mnu file and .iso file in the \_ISO\BACKUP\Utility folder, the menu entry will be listed in the BACKUP menu.
If you place the .mnu file and .iso file in the \_ISO\UTILITIES\Utility folder, it will be listed in the UTILITIES sub-Menu.
If you place the .mnu file and .iso file in the \_ISO\UTILITIES_MEMTEST\Utility folder, it will be listed in the UTILITIES - MEMTEST Sub-Sub-Menu.

Look at the instuctions in the .mnu file for help. 
%MFOLDER% will always be set to the \_ISO\xxx folder - e.g. \_ISO\MAINMENU
$HOME$ will always be set to the folder path of the .mnu file - e.g. \_ISO\MAINMENU\MNU

Note: Files with extensions such as .ISO, .IMG, .IMA, .BIN, .GZ may not need a .mnu file - so just copy the ISO file to either the _ISO\MAINMENU folder or _ISO\AUTO folder.

