## Najboljši rezultat

Shranil boš najboljši rezultat, tako da bodo igralci vedeli, kako jim gre.

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
    definiraj preveri najboljši rezultat
    if <(točke :: spremenljivke) > (najboljši rezultat)> potem
        nastavi [najboljši rezultat v] na (točke :: spremenljivke)
    konec
```

\--- /task \---

\--- task \---

Add your new custom block to the Stage script before the end of the script.

![Stage sprite](images/stage-sprite.png)

```blocks3
ko kliknemo na zastavico
nastavi [življenja v] na (3)
nastavi [točke v] na (0)
počakaj dokler ni <(življenja) < (1)>

+ preveri najboljši rezultat :: custom
ustvai [vse v]
```

\--- /task \---

\--- task \---

Play your game twice to check whether your score gets correctly saved as the `high score`{:class="block3variables"}.

\--- /task \---