## Creșteți dificultatea

Acum vei face jocul mai dificil cu cât îl joacă mai mult. Veți face acest lucru făcând ca punctele să apară mai repede și mai repede în timp.

\--- task \---

Create a new `variable`{:class="block3variables"} called 'delay'.

![Stage sprite](images/stage-sprite.png)

\--- /task \---

\--- task \---

Go to the Stage's Scripts area and create a new script that sets the `delay`{:class="block3variables"} variable to `8` and then slowly reduces the value of `delay`{:class="block3variables"} while the game runs.

![Stage sprite](images/stage-sprite.png)

```blocks3
    când flag apasat
    set [întârziere v] până la (8)
    repetare până < (întârziere) = (2)>
        wait (10) secunde
        schimbare [întârziere v] de (-0.5)
    final
```

\--- /task \---

Notice that this code is very similar to the code you would use to create a countdown timer!

Next, use the `delay`{:class="block3variables"} variable in the code scripts of the 'red', 'yellow', and 'blue' sprites.

\--- task \---

Remove the code block that makes the game wait a random number of seconds between making the dot sprite clones. Replace the block you've removed with your new `delay`{:class="block3variables"} variable:

![screenshot](images/all-dots.png)

```blocks3
<br />- așteptați (alegeți aleatoriu (5) până la (10)) secunde
    așteptați (întârziere :: variabile) secunde
```

Do this for all three dot sprites.

\--- /task \---

\--- task \---

Test the game, and check whether the dots begin to appear more quickly as the game goes on.

+ Acest lucru funcționează pentru toate cele trei puncte colorate?
+ Can you see that the value of the `delay`{:class="block3variables"} variable decreases?

\--- /task \---