# Yosemite San Francisco Font

Replace Helvetica Neue on your 10.10 Yosemite Mac with San Francisco – the Watch font.

The font is adapted from San Francisco – Apple’s new typeface for the Apple Watch. This project was inspired by jenskutilek’s [Fira System Font Replacement](https://github.com/jenskutilek/FiraSystemFontReplacement). The fonts were generated using dtinth's [Yosemite System Font Patcher](https://github.com/dtinth/YosemiteSystemFontPatcher).

![example](http://wellsosaur.us/Ybic/Example.png)

## How to Install:
1. [Download the zipped font files](https://github.com/wellsriley/YosemiteSanFranciscoFont/archive/master.zip).
2. Copy the 6 font files to `/Library/Fonts` on your Mac. *(protip: press `cmd+shift+g` while in Finder to type the path directly.)*
3. Run `sudo chown root:wheel /Library/Fonts/System\ San\ Francisco*` to set the proper ownership of the font files.
4. Repair Disk Permissions `diskutil repairPermissions /` (for good measure)
5. Log out and log back in to apply the changes.

## How to Uninstall:
1. Navigate to `/Library/Fonts` on your Mac and delete the 6 files starting with `System San Francisco`.
2. Log out and log back in to apply the changes.

## How does it Work?
These San Francisco fonts have a special name table with names identical to those of the system fonts. Because the font folder `/Library/Fonts` takes precedence over the fonts which are in `/System/Library/Fonts`, these specially crafted fonts are used for the user interface instead of the real system fonts. The original system fonts are not deleted or modified in any way.

## Important Notes:
1. I assume no copyright over these fonts.
2. I assume no liability for improper installation or improper use. 
3. You must be a registered Apple Developer to use these fonts. Do not download if you don't have a paid Apple Developer Program account.
4. These fonts will *only* work as Helvetica Neue system replacement fonts. If you attempt to use them differently, they **will not work**!