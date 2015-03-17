# Powers

- There are 8 different powers.
- You can have a maximum of 4 items of each power.
- You have an infinite supply of powers, but they take different times to be generated.
- When you have 4 items of a power, the item regeneration timer stops and will not resume until you have 3 or less items of that power.

Possible things to play with would be random “starting pack” so the player doesn’t always have to wait for the “good stuff”.

## Bombs

| Regen | Persistence |
| -- | -- |
| 3s | Timer |

- Bombs explode 3 seconds after being placed.
- Bomb explosions stretch out in every direction from its starting tile, until it hits a wall. Explosions do not bend around corners. In other words, they work exactly like max-power bomberman-bombs.
- Any Skull touched by the explosion dies on impact.
- (Visible timer is optional).
- Bombs destroy everything, including Powers.


## Acid Gas

| Regen | Persistence |
| -- | -- |
| 15s | Timer |

**Gas Spread:**
- A gas cloud starts as 1 tile.
- After 1 second, the cloud will make duplicates of itself in the direction of any free tile
- Every 1 second for the next 7 seconds, each Gas tile has a ⅔ chance of creating another Gas in the direction of any free tile.
- Every 1 second for the last 7 seconds, every Gas tile will have an ever-increasing chance of disappearing, culminating in 100%.
- Just make the darn thing expand and then diminish over the course of 15 seconds. This one’s better iterated with in code than plain writing...

**Gas Kill Condition:**
- A Skull must be under the effect of Gas (occupying the same tile as Gas) for 3 consecutive seconds before it is killed by the gas. This timer resets after 1 second on a non-Gas tile.

## Curse

| Regen | Persistence |
| -- | -- |
| 6s | Timer |

- Emits a magic force in a circle with a radius of 4 tiles.
- Field lasts for 4 seconds.
- Any Skull touched by the field will get a Cursed status. (not visible → should they be?)
- Cursed Skulls are permanently “invulnerable” to rituals..


## Poison

| Regen | Persistence |
| -- | -- |
| 10s | Conditional |

- Kills any Skull it comes into contact with.
- Consumed on contact (i.e. it’s a 1-time use)

## Change to Mummy

| Regen | Persistence |
| -- | -- |
| 10s | Conditional |

- Changes Pink to Blue (or Mutated to Blue, or Blue to Blue, or Tiny to Blue)
- Consumed on contact

## Change to Ghoul

| Regen | Persistence |
| -- | -- |
| 10s | Conditional |

- Changes Blue to Pink (or Mutated to Pink, or Pink to Pink, or Tiny to Blue)
- Consumed on contact


## Blockade

| Regen | Persistence |
| -- | -- |
| 6s | Conditional |

- Blocks the path for Skulls.
- Every time it collides with a Skull, it deteriorates. After 4 impacts, the stop sign is destroyed.

## Ghost Skull

| Regen | Persistence |
| -- | -- |
| 25s | Conditional |

- Behaves with same AI as other Skulls.
- Affected by same powers as other Skulls.
- Terminates other Skulls it comes in contact with, except other Mutated Skulls.
- Self-terminates after destroying 5 Skulls.