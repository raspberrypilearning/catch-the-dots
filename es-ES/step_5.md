## Aumenta la dificultad

Ahora vas a hacer el juego más difícil cuanto más tiempo lo juegue el jugador. Harás esto haciendo que los puntos aparezcan más y más rápido con el tiempo.

\--- task \---

Create a new `variable`{:class="block3variables"} called 'delay'.

![Stage sprite](images/stage-sprite.png)

\--- /task \---

\--- task \---

Go to the Stage's Scripts area and create a new script that sets the `delay`{:class="block3variables"} variable to `8` and then slowly reduces the value of `delay`{:class="block3variables"} while the game runs.

![Stage sprite](images/stage-sprite.png)

```blocks3
    al hacer clic en bandera verde
  dar a [retraso v] el valor (8)
  repetir hasta que < (retraso) = (2)>
    esperar (10) segundos
    sumar a [retraso v] (-0.5)
  end
```

\--- /task \---

Notice that this code is very similar to the code you would use to create a countdown timer!

Next, use the `delay`{:class="block3variables"} variable in the code scripts of the 'red', 'yellow', and 'blue' sprites.

\--- task \---

Remove the code block that makes the game wait a random number of seconds between making the dot sprite clones. Replace the block you've removed with your new `delay`{:class="block3variables"} variable:

![screenshot](images/all-dots.png)

```blocks3
<br />-  esperar (número aleatorio entre (5) y (10)) segundos
    esperar (retraso :: variables) segundos
```

Do this for all three dot sprites.

\--- /task \---

\--- task \---

Test the game, and check whether the dots begin to appear more quickly as the game goes on.

+ ¿Funciona para los tres puntos de colores?
+ Can you see that the value of the `delay`{:class="block3variables"} variable decreases?

\--- /task \---