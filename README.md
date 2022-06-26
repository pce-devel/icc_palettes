# ICC versions of Mednafen PCE Palettes

The included ICC profiles are based on the ongoing work done by the PCE community to approximate what the PCE/TG16 hardware would output for a YUV signal. (Here's a good write-up of how we got here https://www.retrorgb.com/pc-engine-palette-improvements-the-amazing-people-behind-the-technology.html)

## How to use:

Place these ICC Profiles in the following locations on your macOS or Windows system and relaunch your ICC compatible application of choice and they should show up in the respective application menu where ICC files are used.

## <b>macOS:</b><br>
Place the ICC file either in the system `HD_name/Library/Colorsync/Profiles` folder or in the user equivalent located at `HD_name/users/your-username/Library/Colorsync/Profiles` folder (also referred to as:`~/Library/Colorsync/Profiles` in the terminal).

## <b>Windows:</b>
Windows requires the ICC profiles to exist in different folders depending upon the Windows OS version used.

Windows 7 and newer: `DriveLetter:\Windows\system32\spool\drivers\color`<br>
Windows XP: `DriveLetter:\Windows\system32\spool\drivers\color`<br>
Windows 2000/ME: `DriveLetter:\WinNT\system\spool\drivers\color`<br>

The provided ICC profiles in the `icc` folder are as follows :
-  `pce.pal.original.081321.icc` : A v4.2.x ICC Profile based on the Original (dated 081321) commit to Kitrinx's TG16 Palette repository representing the community's initial results as referenced in the above retrorgb article and the relevant GH Repo commit (https://github.com/Kitrinx/TG16_Palette/commit/c29160497d2f02e5f54f4d76a64641c829b46a4c)

-  `pce.pal.kitrinx.041222.icc` : A v4.2.x ICC profile based on the latest (dated 041222) commit to Kitrinx's TG16 Palette repository found here: https://github.com/Kitrinx/TG16_Palette


It is assumed that the user is aware of how to use ICC profiles in their application of preference. 

The provided ICC profiles assume a reference display calibrated using the sRGB IEC61966-2.1 standards assumptions and that the corresponding ICC Display profile transform is already contained within these ICC Profiles.

Due to the wide variety of applications out there that can support ICC profiles, and the multitude of workflows on how to use them correctly, we will refrain from stating that here. Any issues opened about how to use the provided ICC profiles will unfortunately be closed.

The ICC Profiles in this repo are provided as-is, with no implied accuracy, warranty or use-requirement statements thereof.
