# UnrealPakSwitch

## About
#### Author this instrument - Masagrator

Original Themes (All questions are there): 

https://gbatemp.net/threads/how-to-unpack-and-repack-unreal-engine-4-files.531784/

What you need to download:
- Package "UnrealPakSwitchv10.zip" and unpack it.
- Notepad++ (or any other text editor with Perl regular expressions)
- Python 2 or 3
- Unreal Engine:
  - 4.19.2 (for v4 *.pak),
  - 4.20.3 (for v5 *.pak),
  - 4.21.2 (for v7 *.pak),
  - 4.22.3 (for v8 *.pak),
  - 4.24.3 (for v8.23 *.pak),
  - 4.25.4 (for v9 *.pak),
  - 4.26.2 (for v11 *.pak),
  - 4.27.2 (for v11.27 *.pak).

### Additional note
If you want to extract PAK, download just newest version (Unreal Engine 4.27.2) since UnrealPak unpacking is backwards compatible (only exclusion is that v11 PAKs are not fully supported by v11.27 unrealPak).
For packing files usually you can use unrealPak version that matches your PAK version or older, so you can use oldest Unreal Engine 4 (4.19.2) to pak your mods and it should work for 99% of cases.
Remember that's not a rule since developers can change how PAKs are packed or read individually.

## How to use
If you know what version you have, then drag and drop your *.pak file to

>version 4 - "unpack-v4.cmd"
>
>version 5 - "unpack-v5.cmd"
>
>version 7 - "unpack-v7.cmd"
>
>version 8 - "unpack-v8.cmd"
>
>version 8.23 - "unpack-v8-23.cmd"
>
>version 9 - "unpack-v9.cmd"
>
>version 10 - "unpack-v11-27.cmd" (because 10 is unofficial version, we can use as newest tool as possible for Oodle support)
>
>version 11 or 11.27 - "unpack-v11.cmd" or "unpack-v11-27.cmd" (this is because UE 4.27 made breaking changes to pak files without changing header struct, which makes it impossible to differentiate between 11 and 11.27 from header alone).

## Check version of package
The archives are located:
_Game Name/Content/Packs/ as *.pak files *.pak_

1. Copy *.pak file you want to check to unpacked UnrealPakSwitch folder.
2. Drag and drop your file to "1. check.cmd"
It will show:

>Version: X

Where X is a version of your package.
