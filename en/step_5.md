## Increasing the difficulty

Let's make the game get more difficult the longer the player survives, by slowly reducing the delay between dots appearing.

--- task ---
Create a new variable called `delay`{:class="blockdata"}.

![Stage sprite](images/stage-sprite.png)
--- /task ---

--- task ---
On your stage, create a new script that sets the delay to eight seconds, and then slowly reduces the delay time the longer the game goes on.

![Stage sprite](images/stage-sprite.png)

```blocks
	when flag clicked
	set [delay v] to (8)
	repeat until < (delay) = (2)>
		wait (10) secs
		change [delay v] by (-0.5)
	end
```
--- /task ---

Notice that this is very similar to how a game timer works!

You need to use this `delay`{:class="blockdata"} variable in your red, yellow and blue dots' scripts.

--- task ---
Remove the code that waits a random number of seconds between creating clones, and replace it with your new `delay`{:class="blockdata"} variable:

![screenshot](images/all-dots.png)

```blocks
	- wait (pick random (5) to (10)) secs
	wait (delay) secs
```

Do this for all three dot sprites.

--- /task ---

--- task ---
Test the game and see whether the dots begin to appear more quickly as the game goes on.

+ Does this work for all 3 coloured dots?
+ Can you see the value of the `delay`{:class="blockdata"} variable reducing?
--- /task ---
