## Collecting dots

Let's add some dots for the player to collect with their controller.

--- task ---
Create a new sprite called 'red'. This sprite should be a small red dot.

![Red dot sprite](images/dots-red.png)

[[[generic-scratch-draw-sprite]]]

--- /task ---

--- task ---
Add this script to your 'red' dot sprite, to create a new dot clone every few seconds:

![Red dot sprite](images/red-sprite.png)

```blocks
	when flag clicked
	hide
	wait (2) secs
	forever
		create clone of [myself v]
		wait (pick random (5) to (10)) secs
	end
```
--- /task ---

If you click the green flag now you will not see anything happening because all of the cloned sprites appear in the same place.

When each clone is created, you want it to appear in one of the 4 corners of the stage.

![screenshot](images/dots-start.png)

--- task ---
Create a new list called `start positions`{:class="blockdata"} and click the `(+)` to add in the values `-180` and `180`.

![Red dot sprite](images/red-sprite.png)

![screenshot](images/dots-list.png)
--- /task ---

Notice that the coordinate for each corner is some combination of 180 and -180. You can use your list to pick a random corner of the stage.

--- task ---
Add this code to the 'dot' sprite, so that each new dot clone moves to a random corner and then slowly moves towards the controller.

![Red dot sprite](images/red-sprite.png)

```blocks
	when I start as a clone
	go to x: (item (random v) of [start positions v]) y: (item (random v) of [start positions v])
	point towards [controller v]
	show
	repeat until <touching [controller v]?>
		move (1) steps
	end
```

--- /task ---


The code above chooses either `-180` or `180` for the x _and_ y positions, meaning that each clone starts in one corner of the stage.

--- task ---
Test your project. You should see lots of red dots appear in each corner of the screen, and move slowly towards the controller.

![screenshot](images/dots-red-test.png)
--- /task ---

--- task ---
Create 2 new variables called `lives`{:class="blockdata"} and `score`{:class="blockdata"}.

--- /task ---

--- task ---
Add code to your stage to set the `lives`{:class="blockdata"} to 3 and the `score`{:class="blockdata"} to 0 at the start of the game.
--- /task ---


You need to add code to the end of your red dot's `when I start as a clone`{:class="blockcontrol"} code, so that either 1 is added to the player's `score`{:class="blockdata"} if the colours match, or 1 is taken from the player's `lives`{:class="blockdata"} if the colours don't match.

	```blocks
		move (5) steps
		if <touching color [#FF0000]?> then
			change [score v] by (1)
			play sound [pop v]
		else
			change [lives v] by (-1)
			play sound [laser1 v]
		end
		delete this clone
	```

+ Add this code to the end of your stage's script, so that the game ends when the player loses all of their lives:

	```blocks
		wait until <(lives) < [1]>
		stop [all v]
	```

+ Test your game to make sure this code works as expected.
