# WinBif

**WinBif** is a small utility program for handling Infinity Engine bif  files. The bif file format is used with a number of games: Baldurs Gate,  Baldurs Gate: Shadows of Amn, Baldurs Gate: Throne of Bhaal, Icewind  Dale I & II and Planescape Torment. All versions of these games from  GOG.com, Steam, Beamdog, other online providers or from original retail  CD/DVDs are supported.

- Baldurs Gate
- Baldurs Gate: Tales of The Sword Coast
- Baldurs Gate: Siege of Dragonspear
- Baldurs Gate II: Shadows of Amn
- Baldurs Gate II: Throne of Bhaal
- Icewind Dale
- Icewind Dale: Trials of the Luremaster
- Icewind Dale: Heart of Winter
- Icewind Dale II
- Planescape Torment

![img](/images/winbif/bg1.png) ![img](/images/winbif/bgsod.png) ![img](/images/winbif/bg2soa.png) ![img](/images/winbif/bg2tob.png) ![img](/images/winbif/iwd1.png) ![img](/images/winbif/iwd1how2.png) ![img](/images/winbif/iwd2.png) ![img](/images/winbif/pst.png)

**New**: WinBif can now handle bif files (and rim, erf, mod, hak, nwn files) from other games: Jade Empire, The Witcher, Star Wars Knights of The Old Republic I & II and Neverwinter Nights.

![img](images/winbif/witcher1.png) ![img](images/winbif/witcher2.png) ![img](images/winbif/kotor1.png) ![img](images/winbif/kotor2.png) ![img](images/winbif/je.png) ![img](images/winbif/nwn.png) ![img](images/winbif/da1.png) 

**Features:**

- View bif file contents, showing the resource name, type, index, locator and offset to data for file and tile entries.
- Extract single or multiple selections of files stored in bif file to a specified folder.
- Will try to automatically link to a chitin.key file to read resource name entries for a particular bif file.
- Filter current list view by resource types.
- Simulates file names for bif files that don't have a corresponding chitin.key file (or one that can't be located)
- Opens  compressed bifs/cbfs. Supports BIF V1.0 and BIFCV1.0 compression  formats, automatically decompressing files as they are opened.
- Opens rim, erf, mod, hak, nwm archive formats for listing content or extraction.
- Windows explorer shell context menus for opening & extracting bif, rim and erf archives.

## Notes

The latest version of **WinBif** is *v1.0.1.2*

Last Updated On **03/04/2016**

**WinBif** is a 32bit program for:

- Windows XP
- Windows Vista
- Windows 7 (32bit & 64bit)
- Windows 8 (32bit & 64bit)

**WinBif** will create a `WinBif.ini` file in the a specific folder depending on your operating system:

-  **Win 2K/NT/XP**: current folder that the `WinBif.exe` is ran from
-  **Windows Vista**: `C:\Documents & Settings\<Your Username>\Application Data\WinBif` folder
-  **Windows 7**: `C:\Users\<Your Username>\AppData\Roaming\WinBif` folder

All settings can be modified by the options dialog or by directly editing the `WinBif.ini` file.

## Downloads

- [WinBif Readme](\release\apps\winbif-readme.txt?raw=true)
- [WinBif Setup](\release\apps\winbif-setup.exe?raw=true)
- [WinBif Help](\release\apps\winbif.chm?raw=true)