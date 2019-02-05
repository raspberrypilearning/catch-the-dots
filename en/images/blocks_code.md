Due to an issue with the project site this code doesnt work as the line is too long and gets cropped.
```blocks3
	when I start as a clone
	go to x: (item (pick random (1) to (2)) of [start positions v]) y: (item (pick random (1) to (2)) of [start positions v])
	point towards (controller v)
	show
	repeat until <touching (controller v)?>
		move (1) steps
	end
```