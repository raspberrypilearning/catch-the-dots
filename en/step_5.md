## Increasing the difficulty

Let's make the game get more difficult the longer the player survives, by slowly reducing the delay between dots appearing.



+ Create a new variable called `delay`{:class="blockdata"}.

+ On your stage, create a new script that sets the delay to a high number, and then slowly reduces the delay time.

	```blocks
		when flag clicked
		set [delay v] to (8)
		repeat until < (delay) = (2)>
			wait (10) secs
			change [delay v] by (-0.5)
		end
	```

	Notice that this is very similar to how a game timer works!

+ Finally, you can use this `delay`{:class="blockdata"} variable in your red, yellow and blue dots' scripts. Remove the code that waits a random number of seconds between creating clones, and replace it with your new `delay`{:class="blockdata"} variable:

	```blocks
		wait (delay) secs
	```

+ Test your new `delay`{:class="blockdata"} variable, and see whether the delay between dots reduces slowly. Does this work for all 3 coloured dots? Can you see the value of the `delay`{:class="blockdata"} variable reducing?



