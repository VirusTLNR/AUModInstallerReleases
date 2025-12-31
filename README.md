# AUModInstallerReleases
Public facing repository for "AUModInstaller". All source code is private, this is purely for releases, issues, and suggested additions/changes.

## Among Us Versions this works on
- (x86)STEAM - <b>YES</b>
- (x86)ITCH.IO - PARTIAL++ (if TOU-MIRA is anything to go by)
- (x64)EPIC - NO
- (x64)MSSTORE - NO
- (other)MACOS - NO
- (other)LINUX - NO
- (mobile)ANDROID - NO
- (mobile)IOS - NO

++ NOTE - this program only supports STEAM for now, but if the mod in question uses the same files downloaded as steam, then this will work if you disable "install vanilla client" and add the vanilla client yourself.

## Features
- Auto copying of vanilla client from steam library folder (hoping later to actually allow selection of version to download from steam)
- Auto download and installation of ROLES mods from their respective github releases area **
- Auto download and installation of ADDON mods like LevelImposter, Submerged Map and others, from their respective github releases area **
- (WIP) In-program updates when a new version is available downloaded from the releases section of this git (probably available from v0.0.1 onwards) **

** Note: this program uses github API, github api has usage limits (60 requests per hour), this means if you use the program too much within 1 hour, you will need to wait to use it more.
** Note 2: opening the program uses a lot of rates, but downloading multiple mods only takes a few rates, so as long as you open the program once and download all you need to in one go, you should be fine, if you get alerts saying you cant download mods, then wait an hour, and try again. this is a GITHUB API limit, not much I can do unless I can improve how the program works. for the average user, there should be no issue with this limit on a day to day basis.

## How to use
1. make sure you have the latest version of the program. if in a zip, extract to a folder and run the exe. if already unzipped, just run the exe.
1. when you run the program, you will be provided with several drop down boxes and tick boxes, for the ROLES, select the mod + the version.
1. after selecting the ROLES mod + version, tick the boxes for the addons you desire to include in your installation and select the correct version to go with your ROLES mod.
1. if you require a version of vanilla among us that is not the one currently installed, please UNTICK the "install vanilla client" checkbox. You will need to get the vanilla files yourself.
1. once all mods and versions are selected correctly.. select the folder you wish them to be installed to, then click install.
1. now browse to the folder you selected, and you will see the mod is installed there, you can use the same folder for all your mods, or install to different folders, but be aware.. each time you press the INSTALL button, it will delete the install folder, and re-do everything, which could lead to lost settings (some mods save the settings in the bepinex folder) so i would advise installing to a new folder.

## Get a mod added to the program
If you are a mod developer, or anyone really, and you want to see a mod added to the program, either...

Raise an ISSUE on this repository with the github of the mod you wish to be added.

OR..

Alternatively, you can copy one of the ModData JSON files from the "ModData" folder, edit it to include your mod information, and open a PR with the JSON file for the new mod attached.

In both cases, if I approve of the mod being added, I will merge the PR and include the mod and it will show up the next time the program is opened, otherwise I will decline and explain why (or what would need changing for example).