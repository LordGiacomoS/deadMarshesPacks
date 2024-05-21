## To-Do

- [X] Make sure resource pack is compatible with 1.20.6
- [X] Set up biome datapack for mob spawning
- [X] Replace drowned textures in resource pack because orcs (zombies) might convert to drowned and need to be consistent
- [ ] Replace zombie, drowned, and stray sounds with orc sounds?
    - [X] standardize strays & drowned be same as zombie sounds
- [X] Investigate whether I can make petrified slabs actually be mined with shovel (limitation 1)
    - [X] figure out relevant components that need modifying
    - [X] add components to crafting recipes for all tiers of relevant tool
    - [X] add relevant stonecutter/crafting table recipes for the modified block
    	- [X] recipes unlock like expected
    	- [X] can break down log items into planks
    - [X] try to make breaking & walking sounds correct (limitation 2)
    - [X] check for other blocks that should get similar treatment
    	- [X] nether brick stairs
    	- [X] nether brick slabs
    	- [X] nether brick fences
    	- [X] nether brick walls
    - [X] Check for any loot chest/mob dropped tools that would need to be modified in order to be consistent
    	- [ ] Double-Check loot chests in map
    	- [X] Mob Drops (limitation 3)
- [X] Lang file adjustments
- [ ] Create OptiFine/EntityModelFeatures reliant version of mobs that gives more depth? (can be done later as addon)

### Limitation Notes:
1. Cannot find way to make dirt slab & nether brick stuff have correct breaking speed/drops for empty hand (at least without implementing complex functions) -- need to double-check game code in case I'm missing something
2. Cannot find way to give dirt slabs correct sounds without affecting every other block that uses the stone sound collection
    - ~nether brick~ log items do have correct sounds
4. Zombie iron shovel drop can't be modified b/c loot tables affect loot on death and not what entity spawns with -- so stupid


## Mob spawning modifications
### Naturally spawning enemies
- Orc (Melee): Zombie
- Orc (Archer): Stray
- Spider: Spider

### Dungeon only stuff
- Wraith: Vex
- Wight: Wither Skeleton


### Other Notes
- pillager patrols & phantoms will need to be disabled via gamerule, but no other hostile mobs will naturally spawn in modified swamp biome
- glow squids, bats, and passive mobs are unchanged still
- EQ pack lang file is a custom dialect of english that has to be manually selected

- reason for two different namespaces (`minecraft`, `dagorlad`) in data_pack is due to separation between vanilla content being overriden and additons (the whole setup is slightly janky still)

- in the event that zombie sounds are actually being replaced by orc sounds, the common sound definitions between zombie & a few other mobs (ambient, step, hurt, death) will need to be added to `sounds.json`, ideally alongside a few other mob-specific sounds (e.g. zombie -> drowned noise, drowned water-specific noises) 
