## Tabela wyników

Zachowasz rekord wyniku gry, aby gracze mogli zobaczyć, jak dobrze sobie radzą.

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
    zdefiniuj wynik wysoki wynik
    jeśli <(wynik :: zmienne) > (najwyższy wynik)> a następnie
        ustaw [najwyższy wynik v] na (wynik :: zmienne)
    koniec
```

\--- /task \---

\--- task \---

Add your new custom block to the Stage script before the end of the script.

![Stage sprite](images/stage-sprite.png)

```blocks3
po kliknięciu flagi
ustaw [życia v] na (3)
ustaw [wynik v] na (0)
czekaj do <(życia) < (1)>

+ sprawdź wysoki wynik :: niestandardowy
stop [wszystkie v]
```

\--- /task \---

\--- task \---

Play your game twice to check whether your score gets correctly saved as the `high score`{:class="block3variables"}.

\--- /task \---