Use this theme to gives you a Main menu with Vista, Win7, Win8 specific ISO installs and XP installs all in the Main Menu

Example Main Menu
=================
Install Win7 SP1 32-bit
Install Win8.1 32-bit
DOS Menu    [Ctrl+D]
ubuntu.iso


No '0 set default menu' entry
No Install Windows menu entry
Menu entries are not numbered
Add your own \_ISO\MyBackground.bmp 800x600 bitmap.
It has no messages on startup
If you copy FASTLOAD.YES to the root of the E2B drive then Ctrl+R hotkey will cause a refresh.

INSTRUCTIONS
============

1. Copy MyE2B.cfg to \_ISO

2. If you don't want the BACKUP, UTILITIES and DOS menus, then delete the contents of the \_ISO\BACKUP, DOS and UTILITIES folders

3. Add the MAINMENU\$$xxxx files to \_ISO\MAINMENU and edit the $$AddWin2Main.mnu to match the ISOs that you have - add more entries if you wish

4. Delete (or rename to .txt)
  \_ISO\MAINMENU\ZZZF7BootHdd.mnu 
  \_ISO\MAINMENU\ZZWindowsInstall.mnu
  \_ISO\MAINMENU\ZZF8ReloadMenu.mnu

5. Add you ISOs and payload files to \_ISO\MAINMENU (or \_ISO\Linux or \_ISO\xxxx) as usual
   Windows Install ISOs must go in the correct folder under \_ISO\WINDOWS\xxx as usual.

6. You can remove the the \_ISO\MAINMENU\$$XPxxxx files if you are not going to install XP.


7. As there is no 'Set default menu and timeout' menu entry (due to set DEFMENU=0), if you want to set up defaults for the Main menu
   make a new \_ISO\menu_defaults.txt file and add the following text lines (edit as required)

# set default menu item number
default 3
# set default main menu timeout
timeout -1
#prevent menu number from being displayed in top right of menu
debug 0

8. Edit the MyE2B.cfg file to suit your needs and add your own Background .bmp file.

tip: If you leave just one .xml file in the VISTA or Win7 or SVR2K8 folders, then that will be automatically picked.

