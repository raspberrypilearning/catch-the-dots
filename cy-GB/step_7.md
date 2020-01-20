## Sgôr Uchel

Rwyt ti am arbed y sgôr uchel fel bod y chwareuwyr yn gwybod pa mor dda maent yn ei wneud.

\--- task \---

Create a new variable called `high score`{:class="block3variables"}.

![Stage sprite](images/stage-sprite.png)

\--- /task \---

\--- task \---

Select the Stage. Click on 'My blocks' and create a new custom block called `check high score`{:class="block3myblocks"}.

![Stage sprite](images/stage-sprite.png)

![screenshot](images/dots-custom-1.png)

\--- /task \---

\--- task \---

Add code to your custom block so that the block checks if the current value of `score`{:class="block3variables"} in larger than the value of the `high score`{:class="block3variables"} variable, and then stores the value of `score`{:class="block3variables"} as the new value of `high score`{:class="block3variables"}.

![Stage sprite](images/stage-sprite.png)

```blocks3
    diffinio gwirio sgôr uchel
os <(sgôr :: variables) > (sgôr uchel)> yna 
  gosod [sgôr uchel v] i (sgôr :: variables)
end
```

\--- /task \---

\--- task \---

Add your new custom block to the Stage script before the end of the script.

![Stage sprite](images/stage-sprite.png)

```blocks3
pan fo'r flag werdd yn cael ei glicio
gosod [bywydau v] i (3)
gosod [sgôr v] i (0)
aros hyd at <(bywydau) < (1)>

+ gwirio sgôr uchel :: custom
aros [all v]
```

\--- /task \---

\--- task \---

Play your game twice to check whether your score gets correctly saved as the `high score`{:class="block3variables"}.

\--- /task \---