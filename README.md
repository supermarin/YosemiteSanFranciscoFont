YosemiteSanFranciscoFont
========================

Replace Helvetica Neue on your 10.10 Yosemite Mac with San Francisco – the Watch font.

The font is adapted from San Francisco Display – Apple’s new typeface for the Watch. This project was inspired by jenskutilek’s [Fira System Font Replacement](https://github.com/jenskutilek/FiraSystemFontReplacement).

How to Install:
======================
1. Download the zipped font files: <https://raw.githubusercontent.com/wellsriley/YosemiteSanFranciscoFont/master/SystemSanFrancisco.zip>
2. Copy the 5 font files to `~/Library/Fonts` on your Mac. *(protip: press `cmd+shift+g` while in Finder to type the path directly.)*
3. Log out and log back in to apply the changes.

How to Uninstall:
=====================
1. Navigate to `~/Library/Fonts` on your Mac and delete the 5 files starting with `System San Francisco Display`.
2. Log out and log back in to apply the changes.

How does it Work?
====================
These San Francisco fonts have a special name table with names identical to those of the system fonts. Because the font folder /Library/Fonts takes precedence over the fonts which are in /System/Library/Fonts, these specially crafted fonts are used for the user interface instead of the real system fonts. The original system fonts are not deleted or modified in any way.

I assume no copyright over these fonts, nor any liability for improper installation or improper use. Use of these fonts should conform to Apple’s express copyright and rules.