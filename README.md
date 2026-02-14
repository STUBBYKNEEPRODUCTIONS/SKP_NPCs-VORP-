# SKP_NPCs

SKP_NPCs is a lightweight NPC placer for RedM.

It does one job:
- Spawns configured NPCs when a player is within range
- Despawns them when the player leaves the range

No interactions, no prompts, no targeting, no shops. Just placing NPCs.

## Features
- Proximity-based spawn and despawn (per NPC radius)
- Model validation and load timeout safety
- Optional PlaceEntityOnGroundProperly support
- NPCs are frozen, invincible, non ragdoll, and ignore events

## Requirements
- RedM
- vorp_core (listed as a dependency)

## Installation
1. Put the folder in your resources folder:
   `resources/[FLAGSTONERP]/SKP_NPCs/`

2. Ensure it in your server config:
   `ensure SKP_NPCs`

3. Restart the server or start the resource.

## Configuration

Edit `config.lua`

### NPC Entry Format

```lua
Config.npc = {
  {
    npcmodel = 'U_M_M_NbxGeneralStoreOwner_01',
    coords = { x=-324.48, y=803.58, z=117.00, h=291.75, r=20 },
    placeOnGround = false,
  },
}
