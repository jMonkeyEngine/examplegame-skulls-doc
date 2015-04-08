# Powers

- There are 8 different powers.
- You have an infinite supply of powers, but they take different times to regenerate. Display a timerbar, gray out icon while regenerating, pulsate when ready.
- You can have a maximum of 4 items of each power. When you have 4 items of a power, the item regeneration timer stops and will not resume until you have 3 or less items of that power.

Possible things to play with would be random “starting pack” so the player doesn’t always have to wait for the “good stuff”. 

## Bombs

| Regen | Persistence |
| -- | -- |
| 3s | Timer |

- Bombs explode 3 seconds after being placed.
- Bomb explosions stretch out in every direction from its starting tile, until it hits a wall. Explosions do not bend around corners. In other words, they work exactly like max-power bomberman-bombs.
- Any Skull touched by the explosion dies on impact.
- (Visible timer is optional). *I disagree, something should be visible or audible.*
- Bombs destroy Skulls and other Powers, but not walls.


## Acid Gas

| Regen | Persistence |
| -- | -- |
| 15s | Timer |

**Gas Spread:**
- A gas cloud starts as 1 tile.
- After 1 second, the cloud duplicates itself in the direction of any free adjacent tile
- Every 1 second for the next 7 seconds, each Gas tile has a ⅔ chance of creating another Gas in the direction of any free tile.
- Every 1 second for the last 7 seconds, every Gas tile will have an ever-increasing chance of disappearing, culminating in 100%.
- Just make the darn thing expand and then diminish over the course of 15 seconds. This one’s better iterated with in code than plain writing...

**Gas Kill Condition:**
- A Skull must be under the effect of Gas (occupying the same tile as Gas) for 3 consecutive seconds before it is killed by the gas. The Skull's suffocation timer resets after 1 second on a non-Gas tile.

## Curse

| Regen | Persistence |
| -- | -- |
| 6s | Timer |

- Emits a magic force in a circle with a radius of 4 tiles.
- Field lasts for 4 seconds.
- Cursed Skulls are incable of taking part in rituals from now on.
- Any Skull touched by the field receives Cursed status. (not visible → should they be?) *Yes, any power's effect must be noticable, anything else "has not happened" from the POV of the player.*


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

- Changes Ghoul to Mummy (or Ghost to Mummy, or Mummy to Mummy, or Young to Mummy)
- Consumed on contact

## Change to Ghoul

| Regen | Persistence |
| -- | -- |
| 10s | Conditional |

- Changes Mummy to Ghoul (or Ghost to Ghoul, or Ghoul to Ghoul, or Young to Ghoul)
- Consumed on contact


## Blockade

| Regen | Persistence |
| -- | -- |
| 6s | Conditional |

- Blocks the path for Skulls.
- Every time a Skull collides with Blockade, it deteriorates and becomes more transparent. After 4 impacts, the blockade is destroyed.

## Ghost Skull

| Regen | Persistence |
| -- | -- |
| 25s | Conditional |

- Behaves according to the same AI as other Skulls.
- Affected by same powers as other Skulls.
- Terminates other Skulls it comes in contact with, except other Ghost Skulls.
- Self-terminates after destroying 5 Skulls. It fades away and becomes more transparent every time.