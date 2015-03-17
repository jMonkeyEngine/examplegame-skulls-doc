# Units

## Skull Types

**There are four types of Skull units. 3 are enemies, one is friendly.**

### Mini Skull (enemy)
- Move speed: 3 tiles/s
- Smaller than the average Skull.
- Can not engage in summoning rituals with other Skulls.
- Grey skin.
- After being alive for 8-10 seconds, the Young Skull becomes either a Blue or Pink Skull, picked randomly.

### Mummy Skull (enemy)
- Move speed: 1.5 tiles/s
- Normal sized Skull.
- Can engage in summoning ritual with Pink Skulls.
Blue skin.

### Ghoul Skull (enemy)
- Move speed: 1.5 tiles/s
- Normal sized Skull.
- Can engage in summoning ritual with Blue Skulls.
Purple skin.
- Can summon Mini Skulls when charged.

### Mutated Skull (ally)
- Move speed: 3 tiles/s
- Normal sized Skull.
- Kills other Skulls (except Mutated Skulls)
- Terminates after killing 5 Skulls
- Black skin.
- Same vulnerabilities as all other Skulls.

### Summoning Ritual

When two Skulls of opposite colors cross paths, they will stop to perform a summoning ritual. Each Skull holds position in their respective 1x1 unit for 2 seconds, resulting in a charged Pink Skull.

If the Blue Skull is terminated before 2 seconds have passed, the Pink Skull is not charged.

- During the summoning ritual, Skulls are unable to start rituals with other Skulls that might pass them by during the act. Furthermore...
- … the Mummy Skull is unable to start to rituals for 3 seconds after a ritual. ("after a ritual" being when the 2-second ritual process has finished).
- … the Ghoul Skull is unable to start rituals for 6 seconds after a ritual. (alternatively set it to 2 seconds after finishing spawn-action instead)

## Skull Spawning

### Skull Ritual Spawn
A Charged Skull will spawn a random number of 1-5 Young Skulls 2 seconds after the summoning ritual is finished.
- Young Skulls are spawned in 0.5s intervals
- The Pink Skull will stop for 0.2 seconds for each spawn, but will continue moving between spawns.
- Spawned Young Skulls will immediately start moving in a random direction.

### Game Start
At the start of a game, the map will be pre-populated with 10 Mini Skulls.
5 Mummy type, 5 Ghoul type.

## Skull AI
The Skull will move forward until it hits an impassable object (wall, blockade etc.) or a multiple-choice path. It will then randomly choose to turn left (90), right(90) or back (180), then continue moving forward again.

(Can be made smarter, but Skull AI is intenowerstionally simplistic for both code and gameplay reasons).