=========================================================================================

 README & LICENSE

 WinBif v1.0.1.2 by fearless

 Copyright (c) 2016 www.LetTheLight.in

 All Rights Reserved

 fearless.is.my.name@gmail.com
 www.LetTheLight.in


 This software is provided 'as-is', without any express or implied warranty. In no
 event will the author be held liable for any damages arising from the use of this
 software.

 Permission is granted to anyone to use this software for any non-commercial program. 
 If you use the library / custom control / program in an application, an acknowledgement 
 in the application or documentation is appreciated but not required. 

 You are allowed to make modifications to the source code, but you must leave the
 original copyright notices intact and not misrepresent the origin of the software.
 It is not allowed to claim you wrote the original software. Modified files must have
 a clear notice that the files are modified, and not in the original state. This includes
 the name of the person(s) who modified the code. 

 If you want to distribute or redistribute any portion of this package, you will need
 to include the full package in its original state, including this license and all
 the copyrights. 

 While distributing this package (in its original state) is allowed, it is not allowed
 to charge anything for this. You may not sell or include the package in any commercial
 package without having permission of the author. Neither is it allowed to redistribute
 any of the package's components with commercial applications.
 
 Icons used in this program are Farm-Fresh Web Icons - http://www.fatcow.com/free-icons
 
 Thanks to Sam at the spellholdstudios forum for helping test WinBif
 
=========================================================================================


 ----------------------------------------------------------------------------------------
 WinBif Overview
 ----------------------------------------------------------------------------------------

 WinBif is a small utility program for handling Infinity Engine bif files. The bif file 
 format is used with a number of games: Baldurs Gate, Baldurs Gate: Shadows of Amn, 
 Baldurs Gate: Throne of Bhaal, Icewind Dale I & II and Planescape Torment. 
 All versions of these games from GOG.com, Steam, Beamdog, other online providers or from 
 original retail CD/DVDs are supported.

 Additionally WinBif can now handle bif files (and rim, erf, mod, hak, nwn files) from 
 other games: Jade Empire, The Witcher, Star Wars Knights of The Old Republic I & II and 
 Neverwinter Nights.

 ----------------------------------------------------------------------------------------
 WinBif Features
 ----------------------------------------------------------------------------------------
 
 - View bif file contents, showing the resource name, type, index, locator and offset to 
   data for file and tile entries.
 - Winbif will try to automatically link to a corresponding key file (chitin, main, etc)
   to read resource name entries for a particular bif file.
 - Filtering of current list view by resource types.
 - Extract single or multiple selections of files stored in bif file to a specified folder.
 - Simulates file names for bif files that don't have a corresponding chitin.key file 
   (or one that can't be located)
 - Opens compressed bifs/cbfs. Supports BIF V1.0 and BIFCV1.0 compression formats, and will
   automatically decompressing files as they are opened.
 - Opens rim, erf, mod, hak, nwm archive formats for listing content or extraction.
 - Windows explorer shell context menus for opening & extracting bif, rim and erf archives


 ----------------------------------------------------------------------------------------
 HISTORY
 ----------------------------------------------------------------------------------------

 v1.0.1.2
 --------
 Feature    - Added support for png file format found in v2.0 EE patches.


 v1.0.1.1   
 --------
 Feature    - Added support for menu, lua and ttf file formats found in Siege of 
              Dragonspear and v2.0 EE versions of BG and BGII.

 v1.0.1.0   
 --------
 Feature    - Added support for wide (16 bytes) resource name entries in key files found
              in Jade Empire, SWKotoR I & II, Neverwinter Nights and The Witcher games.
 Feature    - Added support for BIF V1.1 format bif files from The Witcher game.
 Feature    - Added support for opening and extracting RIM V1.0, ERF V1.0, MOD V1.0, 
              HAK V1.0 and NWM V1.0 archive file formats, which are found in other games.
 Feature    - Title bar now shows if opened bif file is compressed (in square brackets).
 Feature    - Main WinBif icon changes color to represent archive type opened.
 Change     - Opening another file whilst one is already processing is prevented. Can 
              close processing file instead, which cancels the current operation. This is
              done to prevent thread deadlocks that could occur previously.
 Feature    - Added icons to support extended list of resource types found in all
              supported archives.
 Feature    - Added support for compressing and decompressing bif files.
 Feature    - Added batch processing dialog for compressing and decompressing bif files.
 Feature    - Added shell extension support for opening/extracting rim and erf archives.
 Internal   - Large bif file support. Bif archives > 538MB up to 4GB (2^32) in size will 
              use internal large bif file mapping functions.
 Internal   - Added support for KEY V1.1 file format found in The Witcher game.
 Internal   - Added wide (16 bytes) resource name support to key library.
 Internal   - Added support for resolving and locating other key files: <bifname>.key, 
              main.key, patch.key and '00' terminated bif filenames (Witcher)
 Internal   - Rewrote opening and closing archives routines to account for new archives.
 Internal   - Added functions for processing and extracting rim and erf archives.
 Internal   - Added functions to verify archive types opened via shell / cmdline.
 Internal   - Re-organised internal bif library to compile seperate objs for future use.
 Internal   - Moved resource handling functions from bif library to seperate res library.
 
 
 v1.0.0.7
 --------   
 Bugfix     - Tiles now extract with proper TIS header included.
 Internal   - Libraries updated in preparation for supporting other KEY/BIF formats.
 
 v1.0.0.6
 --------   
 Bugfix     - Resolved crash related to opening a bif file from explorer.
 Bugfix     - bif opened via command line showed other toolbar buttons that normally are
              disabled (extract button for example) whilst opening & processing bif, this
              could allow user to try to extract bif and possibly crash as a result.
 Feature    - Adjusted logic to find help file location better.
 Feature    - Adjusted command line extract dialog to allow for minimize during operation
 Feature    - Updated various info text relating to extractions and cancelling/aborting.
 
 v1.0.0.5
 --------   
 Bugfix     - Resolved stack corruption exception when closing bif files and/or exiting 
              winbif with a bif file open. Memory pointer to internal structure was being
              overwritten and caused GlobalFree to crash.
 
 v1.0.0.4
 --------   
 Debugging  - Debug version to track nature of stack corruption exception crash.
 
 v1.0.0.3
 --------
 Bugfix     - Fixed issue with directory paths when extracting.
 Installer  - Installer now will only remove previous winbif.ini if it hasn't been 
              modified when performing any updates. Previously it would remove and 
              replace it with a default one thus resetting any user settings back to 
              default. Now it will leave it intact when any upgrades are installed.
 
 v1.0.0.2
 --------
 Bugfix     - Fixed crash when closing a bif file as it was opening and processing.

 v1.0.0.1
 --------
 Bugfix     - Fixed issue that allowed extract via button/menu when filter showed 0 items.

 v1.0.0.0 
 --------
 Release    - WinBif first release.


 ----------------------------------------------------------------------------------------
 HOW TO USE
 ----------------------------------------------------------------------------------------

 Install to a folder of your choice. Once installed you can open bif/cbf files from the
 main WinBif program and also via the windows explorer by double clicking on a bif/cbf
 file. Additionally you can right click on a bif/cbf file for other context menu options.

 Any bugs/problems/issues, comments, feature requests are welcome.

 Enjoy.

 ----------------------------------------------------------------------------------------
 NOTES
 ---------------------------------------------------------------------------------------- 
 WinBif will create a WinBif.ini file in the a specific folder depending on your
 operating system:

 - Windows 2000/NT/XP: current folder that the WinBif.exe is ran from
 - Vista: C:\Documents & Settings\<Your Username>\Application Data\WinBif folder
 - Windows 7: C:\Users\<Your Username>\AppData\Roaming\WinBif folder
 
 All the settings can be changed via the options dialog in the main program.
 
 Here is an example of what the .ini file looks like:
 
 [WinBif]
 AddBifNameToExtractPath=1
 BrowseOpen=1
 BrowseOpenFolder=
 BrowseExtract=1
 BrowseExtractFolder=
 BrowseExtractStyle=0
 ResetFilterOnOpening=1
 ExtractAutoClose=1

 More information about each setting can be found in the options dialog and the help file.




 
=========================================================================================