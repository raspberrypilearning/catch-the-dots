## Den Schwierigkeitsgrad steigern

Jetzt machen wir das Spiel schwieriger, je länger der Spieler es spielt. Das machst du, indem du die Punkte mit der Zeit schneller und schneller erscheinen lässt.

\--- task \---

Create a new `variable`{:class="block3variables"} called 'delay'.

![Stage sprite](images/stage-sprite.png)

\--- /task \---

\--- task \---

Go to the Stage's Scripts area and create a new script that sets the `delay`{:class="block3variables"} variable to `8` and then slowly reduces the value of `delay`{:class="block3variables"} while the game runs.

![Stage sprite](images/stage-sprite.png)

```blocks3
    Wenn die Flagge angeklickt wird
setze [Verzögerung v] auf (8)
wiederhole bis < (Verzögerung) = (2)>
    warte (10) Sekunden
    ändere [Verzögerung v] um (-0.5)
Ende
```

\--- /task \---

Notice that this code is very similar to the code you would use to create a countdown timer!

Next, use the `delay`{:class="block3variables"} variable in the code scripts of the 'red', 'yellow', and 'blue' sprites.

\--- task \---

Remove the code block that makes the game wait a random number of seconds between making the dot sprite clones. Replace the block you've removed with your new `delay`{:class="block3variables"} variable:

![screenshot](images/all-dots.png)

```blocks3
<br />-   warte (Zufallszahl von (5) bis (10)) Sekunden
    warte (Verzögerung :: variables) Sekunden
```

Do this for all three dot sprites.

\--- /task \---

\--- task \---

Test the game, and check whether the dots begin to appear more quickly as the game goes on.

+ Funktioniert das für die Punkte aller drei Farben?
+ Can you see that the value of the `delay`{:class="block3variables"} variable decreases?

\--- /task \---