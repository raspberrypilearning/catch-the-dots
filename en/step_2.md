## Creating a controller

Let's start by creating a controller, that will be used to collect dots.

--- task ---
Open the 'Catch the Dots' Scratch project online at <a href="http://jumpto.cc/dots-go" target="_blank">jumpto.cc/dots-go</a> or download from <a href="http://jumpto.cc/dots-get" target="_blank">jumpto.cc/dots-get</a> and then open if you are using the offline editor.

You should see a controller sprite:

![screenshot](images/dots-controller.png)

--- /task ---

--- task ---
Add some code to turn your controller to the right when the right arrow key is pressed:

```blocks
	when flag clicked
	forever
		if <key [right arrow v] pressed?> then
			turn right (3) degrees
		end
	end
```
--- /task ---

--- task ---
Test out your controller -- it should spin to the right when you press the right arrow key on the keyboard.
--- /task ---
