##Additional Credit:

Furok and Grim Age mod team created the original models and textures used in this mod, I just re-rigged the model and did some other tweaks for use in Valheim. Grim Age is a mod based on Warhammer Fantasy, and as such should be considered a Derivative Work to which Games Workshop holds copyright to. Games Workshop's copyright thus extends to the models and textures used in this mod.

GoldenJude for Blacksmith's Tools, which this mod depends on to ensure that parts of the player body are hidden and don't clip with equipped armor pieces. 

zarboz for adjusting rigging to closer match armature, and for refactoring my code + showing me how to add equipped status effects to the armor.

JotunnLib and ValheimLib developers for their respective libraries, which this mod uses to add the items.

##Description:

Adds Chaos Warrior Armor as a new standalone set of armor to the game. Armor names and descriptions are kept fairly vague and don't outright refer to anything from Warhammer lore, if that matters to you. 

Low-res texture version available in optional files on Nexus. Simply download the Nexus optional file corresponding to the version you're using and overwrite your installed ChaosArmor.dll with it; textures should apply client-side on your end and the rest of the code is up-to-date with the main file.

Recipe crafting, upgrade amounts, and various other settings can now be configured through a config file, ReepusDeepusDelmeepus4902761.ChaosArmor.cfg (look, I thought the plugin GUID had to be *really* unique) - let mod run once to generate cfg file

In-game names are 'Uncanny plate harness', 'Uncanny plate helm', and 'Uncanny plate leggings' for the chest piece, helm, and leggings respectively.

Can be spawned through devcommands with prefab names, see Gear Stats Breakdown for prefab names.

Currently craftable/repairable at a standard Forge (no upgrades required) with Flametal + a variety of other materials.

Base stats are slightly higher than a full set of unupgraded Padded Armor, but the maximum upgrade quality is 8 instead of the usual 4.

Make absolutely sure you install the mod requirements, including Blacksmith's Tools as mentioned at the top of the README.

Huge shoutout to GoldenJude for helping troubleshoot rigging issues on the body, in addition to general contributions to the modding tools that made this possible. Also for helping with texturing details.

Massive thanks to Zarboz for helping finetune the rigging, as well as showing me how to add status effects to the armor.

V5 Additions:

Two new, lower-tier armor sets using stripped-down versions of the main chest piece have been added. Crafting has been changed such that you begin with the bronze-tier armor and eventually reforge it into the final tier version. Should not cause any issues if updating from previous version.

See Gear Stats Breakdown for more details.

##Gear Stats Breakdown

*Showing default crafting/upgrade amounts/stats, can be configured in aforementioned config file

(T1 Bronze Tier, 4 quality levels)

Half plate harness (Prefab name T1ChaosPlateArmor):
- Crafting/Upgrading: At Forge of any level
  - Bronze X20 (+5 for each upgrade)
  - Troll Trophy X1
  - Leather Scraps X9
- 10 base armor, +2 per level
  
Tusk plate helm (Prefab name T1ChaosPlateHelm):
- Crafting/Upgrading: At Forge of any level
  - Bronze X10 (+3 for each upgrade)
  - Boar Trophy X1
- 9 base armor, +2 per level
  
Battered plate leggings (Prefab name T1ChaosPlateLegs):
- Crafting/Upgrading: At Forge of any level
  - Bronze X15 (+3 for each upgrade)
  - Troll Hide X5 (+5 for each upgrade)
  - Leather Scraps X4
- 10 base armor, +2 per level

(T2/3, 6 quality levels)

Three quarters plate harness (Prefab name T2ChaosPlateArmor):
- Crafting/Upgrading: At Forge of any level
  - Iron X50 (+10 for each upgrade)
  - Draugr Elite Trophy X1
  - Freeze Gland X5 (+5 for each upgrade)
  - Half plate harness (any quality level)
- 18 base armor, +2 per level

Fanged plate helm (Prefab name T2ChaosPlateHelm):
- Crafting/Upgrading: At Forge of any level
  - Iron X30 (+5 for each upgrade)
  - Wolf Fang X2
  - Freeze Gland X5 (+5 for each upgrade)
  - Tusk plate helm (any quality level)
- 16 base armor, +2 per level

Refurbished plate leggings (Prefab name T2ChaosPlateLegs):
- Crafting/Upgrading: At Forge of any level
  - Iron X30 (+8 for each upgrade)
  - Freeze Gland X5 (+5 for each upgrade)
  - Battered plate leggings (any quality level)
- 16 base armor, +2 per level


(Final Tier, 8 quality levels - only armor before V5)

Uncanny plate harness (Prefab name ChaosPlateArmorBody):
- Crafting/Upgrading: At Forge of any level
  - Flametal X20
  - Three quarters plate harness (any quality level)
  - Fenring Trophy X1
  - Stone Golem Trophy X1 (+1 for each upgrade)
- 28 Base Armor, +2 per level up to max quality of 8
- +5% Stamina regen
- Frost resistance

Uncanny plate helm (Prefab name ChaosPlateHelm):
- Crafting/Upgrading: At Forge of any level
  - Flametal X8
  - Serpent Trophy X1
  - Fanged plate helm (any quality level)
  - 30 Base Armor, +2 per level up to max quality of 8
  - Wraith Trophy X1 (+1 for each upgrade)
- +10% Health regen

Warped plate helm (Prefab name ChaosPlateHelmAlt):
- Crafting/Upgrading: At Forge of any level
  - Flametal X10
  - Serpent Trophy X5, +2 for each upgrade
  - Uncanny plate helm (any quality level)
  - 30 Base Armor, +2 per level up to max quality of 8
- Poison immunity

Uncanny plate leggings (Prefab name ChaosPlateLegs):
- Crafting/Upgrading: At Forge of any level
  - Flametal X10
  - Fuling Totem X2 (+1 per level)
  - Refurbished plate leggings (any quality level)
- 28 Base Armor, +2 per level up to max quality of 8
- +32 carry weight (negates weight of entire Uncanny Plate armor set)


##Installation:

Unzip file contents into your Valheim install directory, after installing all required mods and their requirements.

##Known Issues:

Some users have reported that, on starting the game, the assetbundle can't be found in the assembly dll; currently investigating this issue, and uncertain of how many users it affects (have not been able to reproduce locally). In the meantime, if you aren't running the game through R2 mod manager, you can check the nexus mod page and download the optional file, which loads the asset bundle as a loose file directly from the plugins folder.

##Changelog:

7.1.0
- unload assetbundle after mod initialization, should no longer cause Unity crash on game exit

7.0.0
- added alternate final tier helm with mostly same stats as Uncanny plate helm
	- just an altered version of the mesh with a face grill attached
- translations moved from being hardcoded to a json file, side-loaded via Jotunn

6.0.5
- removed dependency on BoneReorder function from JVL/Blacksmith's Tools - model was re-rigged onto the correct armature

6.0.4
- plugin ver. still 6.0.2, version bump just for dependency updates
- adding Thunderstore version of Blacksmith's Tools as dependency

6.0.3
- plugin ver. still 6.0.2, version bump from before was purely for dependency string updates
- removed blacksmith's tools config files; body hiding configuration is handled in-code now
- fixed minor issue with easter egg Reepus/Deepus/Delmeepus set regarding damage modifiers list; set to empty instead of null
- removed equip message for final tier chaos armor, just a personal judgement call
- updated bepinex dependency version
- some minor tweaks to config options and upper limits

6.0.2
- just updating dependency versions to latest; verified basic functionality still works with H&H 

6.0.1
- minor tweak made to ensure armor renders properly in Vulkan (was previously translucent)

6.0.0
- moved recipe configuration to its own json file, ReepusDeepusDelmeepus4902761.ChaosArmor.recipes.json
- max quality of each tier of Chaos Armor made configurable through ReepusDeepusDelmeepus4902761.ChaosArmor.cfg
- reduced default max quality of tier 3 Chaos Armor to 7, since it is currently impossible to get to forge level 8
- bundled cfg file with this release to replace the old one and its outdated fields

5.0.2
- removed jump/run stamina use modifiers on chest entirely as they did not seem to be working as intended

5.0.1
- changed eye color of T1 and T2 helmets on a suggestion
  - T1 has blue eyes
  - T2 has green eyes
  - Final tier retains original red eyes
- fixed issue in high res textures where they were accidentally left with no filter

5.0.0
- added two lower tiers of stripped-down armor, beginning at bronze
- new crafting recipes requires beginning with the bronze tier armor and reforging it up to the final tier
- final tier upgrade/craft recipes adjusted slightly, but existing crafted sets from previous versions will remain at their quality level

4.0.2
- not an actual update, just adding a very important note about copyright in the description and readme
- actual file contents are the same as 4.0.1, the .dll version is also still 4.0.1 for network compatibility purposes

4.0.1
- added cold resist to chestpiece
- rebuilt assembly from new project yet again
- low res texture version available on Nexus, just overwrite ChaosArmor.dll with the .dll provided in that optional file; texture replacement should be client-side and the rest of the code is up-to-date with main file

4.0.0
- added frost resist to chestpiece
- added new config options
- rebuilt dll from new project, praying to god this stamps out any assembly loading issues; will retain loose assetbundle version on Nexus for some time in case not
- low res texture version available on Nexus, just overwrite ChaosArmor.dll with the .dll provided in that optional file; texture replacement should be client-side and the rest of the code is up-to-date with main file

3.0.2
- changed AssemblyTitle of compiled assembly, was using non-unique name previously

3.0.1
- changed to GetExecutingAssembly in code for loading assetbundle
- fixed minor bug from last version where status effects on chest and legs were not applying

3.0.0
- bumped major version for stricter compatibility enforcement (should've done so last update already tbh)
- changed code class name to hopefully fix assembly loading issues
- added icons for status effects

2.2.4
- added configuration file allowing for adjustment of crafting/upgrade amounts

2.2.3
- added rigging for fingers; still a little rough around the edges, but seems fine in most cases

2.2.2
- added normal and metallic maps for models
- small tweaks to recipe requirements
- made the eyes of helmet faintly emissive
- changed casing on in-game item names to be consistent with vanilla item names
- made some very minor rigging tweaks to the neck parts of model

2.2.1
- fixed bug where equipping chest piece would wipe out player model textures (face, skin, eyes etc.)

2.2.0
- adjusted recipe/upgrade amounts to be more varied
- small mesh adjustments:
  - covered up a small gap between the right arm and breastplate with filler material
  - positioned helmet further forward to closer match player character posture (no longer clips with head in character select screen)
- bunch of cool changes courtesy of zarboz
  - mesh rigging of body matches player posture much better now - unfortunately not enough to prevent clipping, hence Blacksmith's tools remains a requirements
  - on-equip status effects with a special cheesy message for each armor piece, see Gear Stats Breakdown for more details

2.0.1:
- assetbundle now in .dll as an embedded resource, should work when running from mod managers now