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
| HaulerZombieWorkerSetNbtHaul0TaskVariables | Sets the NBT variables for hauling task 0 |
| HaulerZombieWorkerSetNbtHaul1TaskVariables | Sets the NBT variables for hauling task 1 |
| HaulerZombieWorkerSetNbtHaul2TaskVariables | Sets the NBT variables for hauling task 2 |
| HaulerZombieWorkerSetNbtHaul3TaskVariables | Sets the NBT variables for hauling task 3 |
| HaulerZombieWorkerSetNbtHaul4TaskVariables | Sets the NBT variables for hauling task 4 |
| HaulerZombieWorkerSetNbtHaul5TaskVariables | Sets the NBT variables for hauling task 5 |
| HaulerZombieWorkerSetNbtHaul6TaskVariables | Sets the NBT variables for hauling task 6 |
| HaulerZombieWorkerSetNbtHaul7TaskVariables | Sets the NBT variables for hauling task 7 |
| HaulerZombieWorkerSetNbtHaul8TaskVariables | Sets the NBT variables for hauling task 8 |

## Forge NBT
| Name | Use |
| --- | --- |
| minethrallsEntityID | Used for storing tasks for entities |
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
| minethrallsGoToStart | Tells the entity to go to the start position |
| minethrallsGoToEnd | Tells the entity to go to the end position |

## Config
### Hauler Tasks
Task Location: "/config/minethralls/entities/zombies/workers/{minethrallsEntityID}/jobs/haul/#.json"
| Name | Use | Example |
| --- | --- | --- |
| start_item | The item registry for the start item |  |
| end_item | The item registry for the end item |  |
| end_task | The task to preform if the task completes | haul.0 |
| fail_task | The task to preform if the task failed | haul.8 |
| start_pos_x | The X position of the start block. |  |
| start_pos_y | The Y position of the start block. |  |
| start_pos_z | The Z position of the start block. |  |
| end_pos_x | The X position for the end block. |  |
| end_pos_y | The Y position for the end block. |  |
| end_pos_z | The Z position for the end block. |  |
