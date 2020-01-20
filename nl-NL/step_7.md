## Topscore

Je gaat de hoogste score van het spel opslaan, zodat spelers kunnen zien hoe goed ze het doen.

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
    definieer controleer topscore
als <(score) > (topscore)> dan 
maak [topscore v] (score)
end
```

\--- /task \---

\--- task \---

Add your new custom block to the Stage script before the end of the script.

![Stage sprite](images/stage-sprite.png)

```blocks3
wanneer groene vlag wordt aangeklikt
maak [levens v] (3)
maak [score v] (0)
wacht tot <(levens) < (1)>

+ controleer topscore
stop [alle v]
```

\--- /task \---

\--- task \---

Play your game twice to check whether your score gets correctly saved as the `high score`{:class="block3variables"}.

\--- /task \---