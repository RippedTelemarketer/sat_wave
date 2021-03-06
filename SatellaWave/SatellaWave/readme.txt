﻿SatellaWave 0.3.1 (2018-01-09)
by LuigiBlood

This software can make Satellaview compatible server binary files.
A tree of channels is managed by the user and it is possible to save, then load a repository of channels with all their attributes.
You can then export to binary files compatible with SNES emulators that supports them.

As of this time of writing, the SNES emulators that supports such files are:
- bsnes-plus v073+3 and later (in bsxdat folder)
- SNES9X 1.55 and later (in SatData folder by default)

However, the bigger files to be downloaded are only supported in development versions from LuigiBlood, so you may have to compile those versions yourself (repositories can be found at https://github.com/LuigiBlood).

Currently supported channels:
- Message Channel
- Town Status
- Directory
	- Folders
		- Files (also Include Files)
		- Items
- Patch
- Time Channel (BS-X - Global)
- Time Channel (Game Specific)
- Shigesato Itoi no Bass Fishing No. 1 Contest Channels

Changelog:
0.3.1 (2018-01-09)
- Prevent Folder and File Descriptions to be too long.
- Automatically select the recommended file destination after browsing the file.
- BS-X Patch Support (Official BS-X Update & Custom Patches)
- Warn User if Software Channel and/or Logical Channel already exists after editing the channel.
- Software Channel detection now detects Directory.
- Before Export, Repository will be checked for conflicts.

0.3 (2018-01-05)
- Fix CheckUsedLCI() which didn't take into account directories themselves (fixes hang in BS-X).
- [Special Event] is now [Hydrant Access].
- Exporting now changes the Town ID and Directory ID. This allows to change the satellite data in real time as it is emulated if you directly export to the folder.
NOTE: As said earlier in the readme, current stable versions of emulators do not support file downloads properly.

0.2 (2018-01-04)
- Prevent User from choosing more than 5 NPCs/Events (with exceptions).
- Streamed File signification a little clearer (and prevent use of it).
- Added feedback when the folder/file name is too long.
- Prevent new lines for item descriptions.
- Warn user if BS-X will not react properly to the exported bin files.
- Show Current XML filepath in window title [ToontownLittleCat]

0.1 (2017-12-29)
- Initial release