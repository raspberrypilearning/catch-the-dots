## Gana puntos o pierde vidas

Now you're going to add some dots that the player needs to collect.

\--- task \---

Create a new sprite called 'red'. Este objeto debe ser un pequeño punto rojo.

![Objeto punto rojo](images/dots-red.png)

\--- /task \---

\--- task \---

Agrega este código a tu objeto «rojo» para crear un nuevo clon del objeto cada algunos segundos:

![Objeto punto rojo](images/red-sprite.png)

```blocks3
    when flag clicked
    hide
    wait (2) seconds
    forever
        create clone of (myself v)
        wait (pick random (5) to (10)) secs
    end
```

\--- /task \---

If you click the green flag now, it looks like nothing is happening. Esto se debe a que todos los objetos clonados están ocultos y aparecen en el mismo lugar.

Vas a agregar código para hacer que cada vez que aparezca un nuevo clon sea en una de las cuatro esquinas del escenario.

![captura de pantalla](images/dots-start.png)

\--- task \---

Crea una nueva lista que se llame `posiciones de partida`{:class="block3variables"}, haz clic en el icono `(+)` de la lista para añadir los valores `-180`{:class="block3variables"} y `180`{:class="block3variables"}.

![Objeto punto rojo](images/red-sprite.png)

![Lista de 180 y -180](images/dots-list.png)

[[[generic-scratch3-make-list]]]

Luego puedes ocultar la lista desmarcando este cuadro:

![Oculta la lista](images/hide-list.png)

\--- /task \---

Observa que la coordenada para cada esquina del escenario es una combinación de `180` y `-180`. Esto significa que puedes usar la lista para elegir una esquina del escenario al azar.

\--- task \---

Agrega este código al objeto «punto» para hacer que cada nuevo clon aparezca en una esquina aleatoria y luego se mueva despacio hacia el objeto mando.

![Objeto punto rojo](images/red-sprite.png)

```blocks3
    when I start as a clone
    go to x: (item (pick random (1) to (2)) of [start positions v]) y: (item (pick random (1) to (2)) of [start positions v])
    point towards (controller v)
    show
    repeat until <touching (controller v)?>
        move (1) steps
    end
```

\--- /task \---

This new code chooses either `-180` or `180` for the x and y positions, meaning that each 'dot' sprite clone starts in a corner of the Stage.

\--- task \---

Prueba tu proyecto. Deberías ver puntos rojos que aparecen en las esquinas del escenario y se mueven despacio hacia el mando.

![captura de pantalla](images/dots-red-test.png)

\--- /task \---

\--- task \---

Crea dos nuevas variables llamadas `vidas`{:class="block3variables"} y `puntaje`{:class="block3variables"}.

![Objeto punto rojo](images/red-sprite.png)

\--- /task \---

\--- task \---

Add code to your Stage to set the `lives`{:class="block3variables"} variable to `3` and the `score`{:class="block3variables"} to `0` at the start of the game. ![Objeto escenario](images/stage-sprite.png)

```blocks3
when flag clicked
set [lives v] to (3)
set [score v] to (0)
```

\--- /task \---

\--- task \---

Agrega este código al final de la secuencia de comandos del escenario para que el juego termine cuando el jugador pierde la última vida:

![Objeto escenario](images/stage-sprite.png)

```blocks3
    wait until <(lives :: variables) < [1]>
    stop [all v]
```

\--- /task \---

El jugador debe ganar puntos por atrapar puntos y debe perder vidas por no atrapar puntos. A dot can only be caught by matching the colour of the controller to the colour of the dot.

\--- task \---

Go back to the 'red' dot sprite's Scripts area to add some code blocks to the end of the sprite's `when I start as a clone`{:class="block3control"} script.

First, make the dot clone `move 5 steps`{:class="block3motion"} so that it overlaps the controller.

Then add code to either add `1` to `score`{:class="block3variables"} if the colour of the dot clone matches the colour of the controller when they touch, or to take `1` away from `lives`{:class="block3variables"} if their colours don't match.

[[[generic-scratch3-sound-from-library]]]

![Objeto punto rojo](images/red-sprite.png)

```blocks3
    move (5) steps
    if <touching color [#FF0000]?> then
        change [score v] by (1)
        play sound (pop v) until done
    else
        change [lives v] by (-1)
        play sound (Laser1 v) until done
    end
    delete this clone
```

\--- /task \---

\--- task \---

Prueba tu juego para asegurarte de que:

1. Pierdes una vida si no haces coincidir un punto con el color correcto
2. You score a point if you match a dot correctly

\--- /task \---