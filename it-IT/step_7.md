## Punteggio alto

Stai per salvare il punteggio più alto del gioco, in modo che i giocatori possano vedere quanto stanno facendo bene.

\--- task \---

Create a new variable called `high score`{:class="block3variables"}.

![Stage sprite](images/stage-sprite.png)

\--- /task \---

\--- task \---

Select the Stage. Click on 'My blocks' and create a new custom block called `check high score`{:class="block3myblocks"}.

![Stage sprite](images/stage-sprite.png)

![screenshot](images/dots-custom-1.png)

\--- /compito \---

\--- task \---

Add code to your custom block so that the block checks if the current value of `score`{:class="block3variables"} in larger than the value of the `high score`{:class="block3variables"} variable, and then stores the value of `score`{:class="block3variables"} as the new value of `high score`{:class="block3variables"}.

![Stage sprite](images/stage-sprite.png)

```blocks3
    define check punteggio alto
    se <(punteggio :: variabili) > (punteggio alto)> poi
        set [punteggio alto v] a (punteggio :: variabili)
    fine
```

\--- /task \---

\--- task \---

Add your new custom block to the Stage script before the end of the script.

![Stage sprite](images/stage-sprite.png)

```blocks3
quando il flag ha fatto clic su
set [lives v] su (3)
set [punteggio v] su (0)
aspetta fino a <(lives) < (1)>

+ controlla high score :: custom
stop [all v]
```

\--- /task \---

\--- task \---

Play your game twice to check whether your score gets correctly saved as the `high score`{:class="block3variables"}.

\--- /task \---