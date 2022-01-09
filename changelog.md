# Natural Progression Changelog (1.16)

## 2.3.2

### Fixed

- Pebble and Twig blocks not waterlogging correctly
- 1 block of Bedrock at Y=1 every 16x16 being removed
- Pebbles / Twigs leaving half of a plant atop them

## 2.3.1

### Fixed

- Pebbles and Twigs not generating
  - I essentially inverted the blacklist on accident

## 2.3.0

### Added

- `twigPlacementBlacklist` and `pebblePlacementBlacklist` options in config
- Config option for all mobs to have a chance to drop a bone

### Fixed

- Cobbled Netherrack and End Stone not dropping themselves
- Netherite Saw not being in the `saws` tag.

### Changed

- **This mod no longer removes tool recipes**. Datapacks are easy and common - learn them!
  - Instead, it only "nerfs" wooden and stone tools, with a handy tooltip to remind you :D

## 2.2.0

- Pebbles are now part of a Forge tag (`forge:pebbles`)
  - This tag is now used for the advancement for getting a pebble
- Pebbles and Twigs now place on snowy grass correctly
- Internal Refactor

## 2.1.0

### Added

- Pebbles and Cobbles for Netherrack and End Stone
- BetterEnd compatability for plank recipes
- New BlockTag for ignoring the Tool Requirements (wood and stone)
  - Stone Blocks use tag `natural-progression:ignored_stone_blocks`
  - Wood Blocks use tag `natural-progression:ignored_wood_blocks`

### Changed

- Pebbles / Twigs now generate by default in the end and nether too

### Fixed

- Pebbles / Twigs generating on the roof of the nether
- Wrong version number in the file 😆

## 2.0.0

### Added

- Compatability for Quark and Create Stones
  These pebbles will only be created and generated if the required mods are installed.
- New saw types:
  - Gold
  - Diamond
  - Netherite (Fire/Lava Proof, crafted in smithing table)
  - Copper (Uses Tag System)
  - Bronze (Uses Tag System)
  - Steel (Uses Tag System)

### Changed

- Renamed "Basic" Saw to Flint
- Renamed "Improved" Saw to Iron
- HUGE internal refactor for easily adding new pebbles in the future :)
  - Same for saws really.. slightly different but pretty much the same

## 1.4.0

### Added

- Compatibility for the new 1.16 Nether Woods -- whoops 🙄
- Compatibility for several modded woods (INFINITELY many thanks to [sargunv's](https://github.com/sargunv-mc-mods/Natural-Progression/tree/data-fixes) data fixes). This includes:

  - Atmospheric
  - Autumnity
  - Biomes O'Plenty
  - Bloomful
  - Botania (livingwood)
  - Endergetic Expansion
  - Oh the Biomes You'll Go
  - Traverse
  - Upgrade Aquatic

- New tags for bypassing the "You cannot break this block without <TOOLTYPE>" message
  - Add any tool/item to the tag `natural-progression:override_axes` to bypass the check for an axe
  - Add any tool/item to the tag `natural-progression:override_pickaxes` to bypass the check for a pick

### Fixed

- Plank recipes being removed for ALL machines/recipes. Now they're only removed

### Changed

- Removed `removeAllPlankRecipes` config option -- everything is datapack powered now thanks to [sargunv](https://github.com/sargunv-mc-mods).

**NOTE**: Mod compatability requires you to configure the Natural Progression Built-In Datapack to have higher priority than all the mods you wish for it to affect.

![See this gif to learn how](https://oitsjustjo.se/i/dncSxTXyK)

## 1.3.0

### Initial Port to 1.16.x!
