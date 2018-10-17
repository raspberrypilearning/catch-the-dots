## More dots

--- task ---
Duplicate your 'red' dot sprite twice, and name the two new sprites 'yellow' and 'blue'.

![screenshot](images/dots-more-dots.png)
--- /task ---

--- task ---
Change the costume of each sprite so it is the correct colour - the 'yellow' sprite should be yellow, and the 'blue' sprite should be blue.
--- /task ---

--- task ---
Edit code for each sprite so that each coloured dot has to match the correct colour on the controller.

![screenshot](images/dots-all-test.png)

--- hints ---
--- hint ---
This is the code you will need to find and alter in each sprite:
```blocks
	if <touching color [#FF0000]?> then
		change [score v] by (1)
		play sound [pop v]
        ...
	end
```
--- /hint ---
--- hint ---
Here is the code for the yellow sprite
```blocks
	if <touching color [#FFFF00]?> then
        ...
	end
```

Here is the code for the blue sprite
```blocks
	if <touching color [#0000FF]?> then
        ...
	end
```
--- /hint ---
--- /hints ---
--- /task ---
