# Yosemite San Francisco Font

Replace Helvetica Neue on your 10.10 Yosemite Mac with San Francisco – the Watch font.

### Disclaimer: 
This repo was originally created by [Wells Riley](https://github.com/wellsriley).

The font is adapted from San Francisco – Apple’s new typeface for the Apple Watch. This project was inspired by jenskutilek’s [Fira System Font Replacement](https://github.com/jenskutilek/FiraSystemFontReplacement). The fonts were generated using dtinth's [Yosemite System Font Patcher](https://github.com/dtinth/YosemiteSystemFontPatcher).

![example](https://raw.githubusercontent.com/supermarin/YosemiteSanFranciscoFont/master/Example.png)

## Easy Install
Run this command from **Terminal.app**:
```bash
ruby -e "$(curl -fsSL https://raw.github.com/supermarin/YosemiteSanFranciscoFont/master/install)"
```

### Manual Install:
1. [Download the zipped font files](https://github.com/supermarin/YosemiteSanFranciscoFont/archive/master.zip).
2. Copy the 5 font files to `/Library/Fonts` on your Mac. *(protip: press `cmd+shift+g` while in Finder to type the path directly.)* **Important note: this is the `/Library/Fonts` folder, not `~/Library/Fonts`.**
3. Run `sudo chown root:wheel /Library/Fonts/System\ San\ Francisco*` to set the proper ownership of the font files.
4. Run `sudo atsutil databases -remove` to clear the OS X Font Cache
5. Repair Disk Permissions `diskutil repairPermissions /` (for good measure)
6. Restart your computer so the changes can take effect.

### How to Uninstall:
1. Navigate to `/Library/Fonts` on your Mac and delete the files starting with `System San Francisco`.
2. Log out and log back in to apply the changes.

### How does it Work?
These San Francisco fonts have a special name table with names identical to those of the system fonts. Because the font folder `/Library/Fonts` takes precedence over the fonts which are in `/System/Library/Fonts`, these specially crafted fonts are used for the user interface instead of the real system fonts. The original system fonts are not deleted or modified in any way.

### Important Notes:
1. I assume no copyright over these fonts.
2. I assume no liability for improper installation or improper use.
3. You must be a registered Apple Developer to use these fonts. Do not download if you don't have a paid Apple Developer Program account.
4. These fonts will *only* work as Helvetica Neue system replacement fonts. If you attempt to use them differently, they **will not work**!
5. While San Francisco “Text” is recommended by Apple for smaller sizes (mainly user interfaces), the “Display” face has much better letterspacing and kerning. If you prefer the Text face, install the files in the “Text Face (alternate)” folder.

### Security
If you're concerned about the authenticity of the `install` script, you can clone this repo and verify the installer with my GPG signature. You should find a file named `install.sig` which you can use to:

* Verify that `install` hasn't been tampered with, and
* Get proof that it really was authored by [Wells Riley](http://wells.ee/pgp).

`$ gpg --recv-key D349C578`

`$ gpg --verify --with-fingerprint install.sig install`

And then verify the resulting signature's fingerprint against Wells Riley's published fingerprint at [http://wells.ee/pgp](http://wells.ee/pgp).
