# Miscellaneous

## Research - Rats!
- http://www.windowsgames.co.uk/rats.html (demo can be played with Wine)
- https://itunes.apple.com/app/rats!-lite/id325823520?mt=8

<iframe width="480" height="360" src="https://www.youtube.com/embed/YnO406cOVmM" frameborder="0" allowfullscreen></iframe>

End.

## Notes

- Game demo will be on Nicolaas de Bruyn’s Google Play account.
- Tutorials (when we get to that point) will be on wiki.jmonkeyengine.org, but could be cross-published (e.g. pitch to tutorials site.)

TODO:

- Proper perspective explanation - [refpic](http://images.g4tv.com/ImageDb3/242124_l/e3-2010-bomberman-live-battlefest-screenshot.jpg)
- clarify “max stock = 4” concept for powers


## Stretch Goals

Stretch Goals
{All random stuff that I’ve written down with no concern for scope whatsoever. The only one I would seriously consider is the responsive menu and the keyboard input}

### Keyboard Input

>My first impression was that I was annoyed that I couldn't scroll around quickly enough, there was always someone spawning in the other corner. ;) I already need the mouse to pick powers, and apply them, and now additional to scroll.
> I wish I could use the keyboard for selecting powers (e.g. numbers) and for scrolling (e.g. arrows). Possibly you didn't add keyboard inputs because you wanted to keep it simple. On the other hand, alternative keyboard input is a standard desktop game feature that people will want to learn about."


### End-game Cinematic

Necromancer comes to fetch his souls (or whatever) and will succeed or fail. (Ruth please share the ideas you had for this sort of thing!) 

>If player wins, the cinematic shows the necromancer at his altar, eyes wide, dropping his latte macchiato, clasping his chest. His unbelieving eyes dart at the spirit-like shells of his Skulls floating up from the floor and popping weakly in midair like soap bubbles, while he shrinks and collapses to his knees. All glow fades, he becomes a mere mortal. Bats and black cats laugh at him.

>In the moment monsters win, the cinematic shows all Skulls stop at the same time. They turn around, and stare straight up into the players eyes and grin. They grow and glow while quickly moving into a symmetric formation along the outline of a star. A cloud of bats appears in their middle out of which the necromancer rises. He grins and also glares up at the player while raising his arms in a welcoming gesture. Everything starts glowing more and more until everything is blindingly white and then -- darkness. 

### Responsive menu to allow horizontal mode

Instead of forcing a horizontal layout with the actions menu on the right, the menu could be moved to the bottom of the screen when in vertical mode.


### Different floor levels
Allow a non-flat map, i.e. there could be a stairway leading up the height of one tile. In this case, bombs would probably not go past the stairway, while gas would still spread through.

### Advanced Skull AI
Advanced enough to simulate more believable rat behavior. Maybe GOAP. Will have a major impact on the gameplay though, but fun for testing.


### Type-sensitive progress bar
Shows how many skulls are left of each type, e.g. by color-coding the bar or a pie chart. 

### Game Remixes
- Different path/grid system.
- Different AI.
- Different UI library.

### Randomly Generated Maps
New maps can be created randomly.

### Alternative grid types

- Sigma Maze (Hexagonal grid)
- Delta Maze (Triangular grid)
- Theta Maze (Circular/freeform grid)


### Combos
- Bombs ignite gas instead of destroying it, making a large but short-lived killing field.
- Radioactivity turns mutated Ghost Skulls into super-mutated Ghost Skulls who use a smarter AI to hunt down Skulls for the player. 
- Zombie-Skulls!.. somehow. Killed Skulls leave twitching remains behind; every Skull passing these remains has an x % chance of reanimating the fallen for a last ritual, after which the zombie turns into a Cursed Skull.