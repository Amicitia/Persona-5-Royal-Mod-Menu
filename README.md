# ATTENTION!
This repository is obsolete and was used for testing the PS4 version of the mod menu.  
See [here](https://github.com/ShrineFox/Persona-5-Mod-Menu/) for the updated one.
# Persona 5 Royal Mod Menu
**Custom scripts for Persona 5 Royal that replace the square button function with a fully featured trainer**
![Image of the menu ingame](https://cdn.discordapp.com/attachments/428021649246388224/447597680018063372/unknown.png)
## Notable Features
- Add Personas, add skills to any party member's currently equipped Persona, delete all Personas currently in the protagonist's stock
- Add points to your stats (Knowledge, Guts, Charm etc.)
- Add a specified quantity of any item, armor, weapon etc.
- Change your rank with any confidant and unlock their abilities instantly
- Change the protagonist's/team's name at any time
- Clip through walls and explore hidden areas
- Load encounters, music, fields, events, animations, and models from filename IDs
- Manipulate the camera (reposition, lock, unlock, rotate, change FOV)
- Toggle the HUD, navigator character, party members, romance flags and more
- Instantly change the current date and weather
- Add Personas and change you or your party members' Skills
## Usage
You can use the [your preferred package manager](https://shrinefox.com/guides/2021/06/21/when-to-use-aemulus-or-mod-compendium/) to build a mod.cpk from the [latest compiled Release](https://github.com/Amicitia/Persona-5-Royal-Mod-Menu/releases) (or your own compiled version, see below).
With [the game patched to load mods on a PS4 capable of running HEN](https://shrinefox.com/guides/2020/09/30/modding-persona-5-royal-on-ps4/), and the mod.cpk placed in /data/p5r/mod.cpk on your PS4, you can use the Mod Menu in-game.
## Compiling
1. Download the latest build of TGE's [AtlusScriptCompiler](https://github.com/tge-was-taken/Atlus-Script-Tools)), which you can use to compile the **.flow** and **.msg** scripts in this repository and recompile them into **.bf** format.
2. Also download [TGE's PAKTools](https://github.com/tge-was-taken/AtlusFileSystemLibrary/releases).
3. Edit the build.bat file with the paths to your AtlusScriptCompiler and PAKTool exe files. Name your edited copy build_local.bat. Place the PAK files from your copy of the game in the input folder.
4. Run build_local.bat.

When you run the bat, the scripts will be compiled into BF files and packed into new PAK files.

There are 4 different scripts that must be recompiled:
- **field.bf** (for the field) found in ps4R.cpk\field\\**fldPack.pac**
- **dungeon.bf** (for palaces) found in ps4R.cpk\field\\**dngPack.pac**
- **at_dng.bf** (for mementos) found in ps4R.cpk\field\\**atDngPack.pac**
- **fscr0150_002_100.bf** (for newgame) found in dataR.cpk\script\\**field**
