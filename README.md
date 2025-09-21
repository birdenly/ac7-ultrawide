# ac7-ultrawide
Mod AC7 to work at ultrawide resolutions.

This is a fork of massimilianodelliubaldini ac7-ultrawide to make it work for Nucleus Co-op Split screen (tested with 1080p/1440p monitors)

Only difference being this version is it accepts the resolution as input (CLI) and a different way to handle the HUD at 8:9 res

What it does:

1. Gets the Resolution from CLI (ex: ac7-ultrawide-for-nucleus.exe (Width) (Height) (1 for vertical split, 0 for not))
    - For the vertical split option: 1 works for 32:9 and 0 for 8:9 aspect ratios
2. Creates a time-stamped backup of the game executable. This is NOT for redistribution!
3. Hex edits the game executable to remove letterboxing (black side bars) and adjust the field of view (FOV).
4. Compares the modified exe against the backup to determine successful hex editing.
5. Modifies the shader files for the correct position and resolution.

WARNING: 

Due to the fact that this mod makes direct modification to the game executable, 
the game's new anticheat system may flag you and get you permanently banned from online play. 
This developer holds no responsibility if this happens to you! 

Installation (Using Nucleus Co-op): 

1. Download Nucleus Co-op
2. Add the game
3. Start the game using Nucleus
4. Everything will be setup for you.
- UltraWide will only apply to the game when started by Nucleus, not steam.

Installation (Manual): 

1. Download the .Zip in [Github releases](https://github.com/birdenly/ac7-ultrawide/releases/tag/release)
2. Place the files in <Steam Installation Location>\SteamApps\common\ACE COMBAT 7.
3. Create a Bat and add the CLI commands (ac7-ultrawide-for-nucleus.exe (Width) (Height) (1 for vertical split, 0 for not))
4. Run it.

Uninstallation:

1. Delete d3d11.dll from your game directory.
2. Delete Ace7Game.exe from your game directory.
3. "Verify integrity of game files" in Steam. This will re-download the most up-to-date executable.




