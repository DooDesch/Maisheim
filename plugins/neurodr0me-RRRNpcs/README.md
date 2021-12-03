# RRR Non-Player Characters

## HUMANS!
- Adds non-player humans to the game.

## CONFIGURE YOUR OWN HUMANS!
- Create new custom NPCs, using the same config system used by my mod [RRR Monsters](https://valheim.thunderstore.io/package/neurodr0me/RRRMonsters/) to configure other, non-human mobs.
- Equip your NPC with any armor or weapon that players can equip, including those from other mods.
- Customize every aspect of your human, from name to faction, exact damage dealt by type (Poison Sword, Lightning Bow) to damage weakness/resistance, items dropped, fine tune AI settings, even change size (Skinny Humans? Elves! Stout Humans? Dwarves!) and add color tinting, and add color particle effects like body-flame and body-smoke (more FX options in future versions). And more!
- Designed to work with other mods that use prefabs, so you can produce custom monsters for use in popular customization mods like Tykea's [Creature Level and Loot Control](https://valheim.thunderstore.io/package/Smoothbrain/CreatureLevelAndLootControl/) or ASharpPen's [Spawn That](https://valheim.thunderstore.io/package/ASharpPen/Spawn_That/) and [Custom Raids](https://valheim.thunderstore.io/package/ASharpPen/Custom_Raids/). 
- Automatically syncs custom monsters with servers, so each server can seamlessly offer a unique experience.


## Notes


- **Note: Alone, this mod only adds the NPCs to the game, but will not cause them to appear in spawn tables or events.**

- **In order to actually encounter NPCs, you will need another mod. My own mod [RRR Better Raids](https://valheim.thunderstore.io/package/neurodr0me/RRRBetterRaids) is already fully configured to work with this mod without extra work.**

- You can also use any other mod that enables custom mob spawns or custom raids, provided you can configure them yourself.
  - I highly recommend ASharpPen's [Spawn That](https://valheim.thunderstore.io/package/ASharpPen/Spawn_That/) and [Custom Raids](https://valheim.thunderstore.io/package/ASharpPen/Custom_Raids/).
    - Prefab IDs for the new NPCs included in this mod are listed below.
    - Prefab IDs for your custom NPCs will follow the format "RRRN_NewPrefabName".

- You can also use any other mod that enables custom mob spawns or custom raids, provided you can configure them yourself. Prefab IDs for the mobs included in this mod are listed below.

#
## Setup

Extract the dll file to your `Valheim\BepInEx\plugins` folder. Config files must be in `Valheim\BepInEx\config` (subfolders are okay). Config files will also be generated automatically if missing.

## Help!

If you need further assistance, feel free to bug me (@neurodr0me) in the Valheim Modding Discord at https://discord.gg/MXqWrn532w

#### Added Prefab IDs
- (Note: T1-T6 refers to progression tiers, Meadows > Forest > Swamp > Mountains > Plains > Endgame)
```
RRR_Hostile_T1
RRR_Hostile_T2
RRR_Hostile_T3
RRR_Hostile_T4
RRR_Hostile_T5
RRR_Hostile_T6
```