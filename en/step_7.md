## High score

Let's save the high score, so that players can see how well they're doing.

--- task ---
Create a new variable called `high score`{:class="blockdata"}.

![Stage sprite](images/stage-sprite.png)

--- /task ---

--- task ---
Click on the stage and create a new custom block called `check high score`{:class="blockmoreblocks"}.

![Stage sprite](images/stage-sprite.png)
![screenshot](images/dots-custom-1.png)

--- /task ---

--- task ---
Add code to your custom block to store the current `score`{:class="blockdata"} as the `high score`{:class="blockdata"} `if`{:class="blockcontrol"} it's the highest score so far:

![Stage sprite](images/stage-sprite.png)

```blocks
	define [check high score]
	if <(score) > (high score)> then
		set [high score v] to (score)
	end
```
--- /task ---

--- task ---
Just before the end of the game, add in your new custom block.

![Stage sprite](images/stage-sprite.png)
```blocks
when flag clicked
set [lives v] to (3)
set [score v] to (0)
wait until <(lives) < (1)>
+ check high score
stop [all v]
```

--- /task ---

--- task ---
Test the code you've added. Play your game to check whether your score gets saved as the `high score`{:class="blockdata"} if it is larger.
--- /task ---
