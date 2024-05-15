## To-Do

- [X] Make sure resource pack is compatible with 1.20.6
- [X] Set up biome datapack for mob spawning
- [ ] Replace drowned textures in resource pack because orcs (zombies) might convert to drowned and need to be consistent
- [ ] Replace zombie and stray sounds with orc sounds?
- [ ] Investigate whether I can make petrified slabs actually be mined with shovel
    - [x] figure out relevant components that need modifying
    - [x] add components to crafting recipes for all tiers of relevant tool
    - [ ] add relevant stonecutter/crafting table recipes for the modified block
    - [ ] try to make breaking & walking sounds correct
    - [ ] check for other blocks that should get similar treatment
    	- [ ] nether brick stairs
    	- [ ] nether brick slabs
    	- [ ] nether brick fences
    	- [ ] nether brick walls
    - [ ] Check for any loot chest/mob dropped tools that would need to be modified in order to be consistent
    	- Zombie iron shovel drop can't be modified b/c loot tables affect loot on death and not what entity spawns with -- so stupid
- [ ] Lang file adjustments
- [ ] Create OptiFine/EntityModelFeatures reliant version of mobs that gives more depth?

## Mob spawning modifications
### Naturally spawning enemies
- Orc (Melee): Zombie
- Orc (Archer): Stray
- Spider: Spider

### Dungeon only stuff
- Wraith: Vex
- Wight: Wither Skeleton


### Other Notes
- pillager patrols & phantoms will need to be disabled via gamerule, but no other hostile mobs will naturally spawn
- glow squids, bats, and passive mobs are unchanged still

