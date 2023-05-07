# Hualer Profession Data
## Procedures
| Name | Use |
| --- | --- |
| HaulerZombieWorkerUpdateTick | Main procedure for most things |
| HaulerZombieWorkerInternalSpawn | Main procedure for the entity when they spawn |
| HaulerZombieWorkerRightClicked | Main procedure for right-click trigger for the entity |
| | |
| | |
| | |
| HaulerZombieWorkerSetNbtTaskVariables | Sets the NBT variables from the config file |
| HaulerZombieWorkerGoToStart | Runs the start position script |
| HaulerZombieWorkerGoToEnd | Runs the end psition script | 

## Forge NBT
| Name | Use |
| --- | --- |
| minethrallsEntityID | Used for storing tasks for entities |
| minethrallsXp | Used for storing experience |
| minethrallsStartInvSize | The start block inventory size of containers |
| minethrallsEndInvSize | The end block inventory size of containers |
| minethrallsStartItem | The item to collect at the start position |
| minethrallsEndItem | The item to store at the end position |
| minethrallsEndTask | The task to preform once the current task is complete |
| minethrallsFailTask | The task to preform if the task can't be completed |
| minethrallsStartPosX | The X position of the start block |
| minethrallsStartPosY | The Y position of the start block |
| minethrallsStartPosZ | The Z position of the start block |
| minethrallsEndPosX | The X position for the end block |
| minethrallsEndPosY | The Y position for the end block |
| minethrallsEndPosZ | The Z position for the end block |
| minethrallsEndCmd | A command to run once the task is complete. |
| minethrallsFailCmd | A command to run when the task fails |
| minethrallsEndXp | The amount of XP to give the entity once the task is complete |
| minethrallsFailXp | The amount of XP to give the entity if the task fails |
| minethrallsGoToStart | Tells the entity to go to the start position |
| minethrallsGoToEnd | Tells the entity to go to the end position |

## Commands
- Owner: The player that tamed the entity.
- Owner Limited: Owner but has limited access.
- Admin: A player with OP command permission level.

| Command | SubCommand | Permission Level |
| --- | --- | --- |
| Debug | useDebug | Admin Level 2 |
| mapProfileName | mapProfileName | Admin Level 2 |
| task | continue/entity | Owner/Admin Level 2 |
| task | set/entity/taskFile/hauler/startSlotSize/startSlotSize | Owner/Admin Level 2 |
| task | set/entity/taskFile/hauler/endSlotSize/endSlotSize | Owner/Admin Level 2 |
| task | set/entity/taskFile/hauler/endXp/endXp | Admin Level 2 |
| task | set/entity/taskFile/hauler/failXp/failXp | Admin Level 2 |
| task | set/entity/taskFile/hauler/endTask/endTask | Owner/Admin Level 2 |
| task | set/entity/taskFile/hauler/failTask/failTask | Owner/Admin Level 2 |
| task | set/entity/taskFile/hauler/startPos/startPos | Owner/Admin Level 2 |
| task | set/entity/taskFile/hauler/endPos/endPos | Owner/Admin Level 2 |
| task | set/entity/taskFile/hauler/startBlock/startBlock | Owner/Admin Level 2 |
| task | set/entity/taskFile/hauler/endBlock/endBlock | Owner/Admin Level 2 |
| task | set/entity/taskFile/hauler/startItem/startItem | Owner/Admin Level 2 |
| task | set/entity/taskFile/hauler/endItem/endItem | Owner/Admin Level 2 |
| task | start/entity/startTask | Owner/Admin Level 2 |
| task | pause/entity | Owner/Admin Level 2 |

## Config
### Hauler Tasks
Task Location: "/config/minethralls/entities/zombies/workers/{minethrallsEntityID}/jobs/haul/#.json"
| Name | Use | Example |
| --- | --- | --- |
| start_item | The item registry for the start item | minecraft:cobblestone |
| end_item | The item registry for the end item | minecraft:cobblestone |
| start_block | The block registry for the start block | minecraft:chest |
| end_block | The block registry for the end block | minecraft:chest |
| end_task | The task to preform if the task completes | 1 |
| fail_task | The task to preform if the task failed | 0 |
| end_cmd | When the task fails it will run a allowed command | /msg NorthWestTrees Hello World! |
| fail_cmd | When the task fails it will run a allowed command | /msg NorthWestTrees Goodbye World! |
| start_inventory_size | The amount of slots the start container block has | 27 |
| end_inventory_size | The amount of slots the end container block has | 9 |
| start_pos_x | The X position of the start block. | 100 |
| start_pos_y | The Y position of the start block. | 64 |
| start_pos_z | The Z position of the start block. | -100 |
| end_pos_x | The X position for the end block. | 90 |
| end_pos_y | The Y position for the end block. | 64 |
| end_pos_z | The Z position for the end block. | -100 |

### Commands.txt
- A list of allowed commands can be used when a task is completed or failed.
- One command per line
- All commands are checked before adding to the entity if it contains the same start string.
