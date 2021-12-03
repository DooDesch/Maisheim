# Forgotten_Biomes

Add some variety in AshLands and DeepNorth biomes
Re-enable the old Mistlands look

## Features

- AshLands and Ashrain will burn if you not in water or have very good fire resist.
- AshLands/Ashrain damage trigger to enable/disable it
- Configurable damage value (Default 10% of your health)
- AshLands have Rocks, Ore, etc.. (Configurable)
- DeepNorth have Rock, Ore, etc.. (Configurable)
- Add Vegetation/rock to all biomes (Configurable)
- Add Location, Tower, Ruin etc.. to all biomes. Some have monsters !  (Configurable)

## DISCLAIMER
Enable every options led to an increased World Generation time, be prepared.
On Server this will increase the packet size.


##WHY ?
Valheim come with a lot of Structure not fully implemented in game, but still available in code.
I just want to re-enable everything and let player choose if it's useful or not;
You can customize biome vegetation and rocks, choose to add more and more things in every biomes.

Ashlands and DeepNorth were empty. now you have (by default) a real biome, with rocks, veins etc..

With addition of Disabled and Hidden Locations, you can try what the dev didn't showed.
Stone tower, Castle, old Pillar, some location are broken, some may collapse when you come closer.
This mod add more diversity in your world.

So now Valheim is a real Old World with fallen realms. And you can customize YOUR VALHEIM !

This mod 

## SPECIALS THANKS
thedefside, NemOmo

## FAQ

- Works on already created world, but change are only available in unexplored/non generated area.
- If uninstalled, everything related to this mod may despawn


## Client / Server

- For Dedicated, need to be installed on BOTH client and Server


#Changelog:
- v0.0.14
	- Removed vegetation not in Mistland by default.
	- Added Vanilla Mistland vegetation to generation
	- Mistlands vegetation is enabled by default
	- Code cleaning
	- Added a CSV file with all Vegetation 
- v0.0.13
	- Updated Mistland default vegetations file (thanks to thedefside on Nexusmods)
	- Updated Linux based server detection with better path writing (thanks to NemOmo on Nexusmods)
- v0.0.12
	- Hearth and Home compatibility Quick Fix
- v0.0.11
	- not released
- v0.0.10
	- MistLands, "Poison Fumes" should be removed with potion even if you're not in the right biome (fix)
	- MistLands, "Poison Fumes" should only be triggered on land (improvement)
	- All "Forgotten Biomes" debuff are removed when you die (improvement)
	- Added two disabled "grass type" to clutter generation in Meadows and Plains (Client Side)
	- Added disabled rooms in Dungeons generation (not recommended yet)
	- Un-removable Locations (Stone Keep, etc.) are now destructible and do not reload (fix) May work on existing locations
	- Tweaked some Location proxy (overall location spawn fix)
	- First shaders implementation, not functionnal, to replace Snow in AshLands by ashes and add Snow in whole DeepNorth)
	- General improvement in world generation speed
	- refactoring
- v0.0.9
	- Added an option to load config from internal var instead of files (Linux based server fix)
	- OS detection on launch to choose better configuration without changing anything
	- Added NexusID form update
- v0.0.8
	- Added "Debug" Trigger to enable more Logs
- v0.0.7
	- BugFix (not released)
- v0.0.6
	- Verbose version
	- Fixed a null exception
	- Refactoring, optimization
- v0.0.5
	- Added Ocean biome Vegetation generation (keep in mind Ocean is -1000 depth).
	- Mistlands: Added "Poison" effect (Configurable), without proper flask you'll die from poisoning.
	- DeepNorth: cold slows down your movements without proper resist/flask).
	- Added configuration file to "remove" Location from world generation.
	- Configurable "Distance from center" for every Locations added with this mod (Default 200).
	- Biomes Status Effect may not interfer with others mods Status Effect
	- Update to reflect Valheim 0.153.2 change.
	- Refactoring

- v0.0.4:
	- Added configuration for Fire resist in Ashland
	- Increased default Damage in Ashland
	- Added Vegeation configuration, choose what you want to spawn.
	- Added all biomes (except Ocean), customize your World.
	- Added Locations generation.
	- Added configuration files to choose Location to spawn.
	- Added "Disabled" Locations to the World generation. (Default off)
	- Added "Hidden" Locations to the World generation. (Default off)
	- Added "Hidden Locations" compliant  integration in their respective Biomes.
	- Removed "FireHole" in AshLands, added proper Surtling location instead.
	- Refactoring
- v0.0.3:
	- Better Vegetation integration, less patch more vegetation
- v0.0.2:
	- Fixed a bug that prevent legit object to spawn in their original biomes
- v0.0.1: 
	- Initial release
	- First attempt just for the fun