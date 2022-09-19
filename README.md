# Description
ZKMod Engine Repair is a Project Zomboid Steam Workshop Mod which lets you define how much a spare engine part repairs and whether to use only one spare engine part from your inventory per repair.

Tested on 41.73. Will not work if you use other mods that override *VehicleCommands.lua*.

Mod page on Steam: https://steamcommunity.com/sharedfiles/filedetails/?id=2759637097

Workshop ID: 2759637097 / Mod ID: ZKModEngineRepair

# Configuration
You may configure or turn features off in *\<servername\>_SandboxVars.lua* or by GUI. If you don't configure anything default values are used.
  
Example configuration:
```
SandboxVars = {
    [...]
    ZKModEngineRepair = {
        Multiplier = 3.0,
        UseOnePartOnly = 1,
    },
}
```
All options and possible values: https://github.com/IkeC/ZKModEngineRepair/blob/master/media/sandbox-options.txt


# Changelog

## ZKMod Engine Repair 1.2 (2022-09-19)

Updated for 41.73
- Cars and trailers can be towed again.
- Options can now be configured in the game GUI.

## ZKMod Engine Repair 1.1.1 (2022-02-26)

Updated for 41.66

## ZKMod Engine Repair 1.1 (2022-02-24)

Multiplier was too strong with when player had a high mechanics skill. It is now applied before the skill bonus is added.

Before: 
With multiplier 3, mechanics skill 5: 3% repair per engine part 
With multiplier 3, mechanics skill 10: 12% repair per engine part 

Now:
With multiplier 3, mechanics skill 5: 3% repair per engine part 
With multiplier 3, mechanics skill 10: 6% repair per engine part 

## ZKMod Engine Repair 1.0 (2022-02-20)

Lets you define how much a spare engine part repairs and whether to use only one spare engine part from your inventory per repair. Multiplier and inventory behaviour can be configured in sandbox settings. If you don't configure anything the multiplier is 3.0, so repairs are three times more efficient, and only one spare engine part from your inventory is used per repair.