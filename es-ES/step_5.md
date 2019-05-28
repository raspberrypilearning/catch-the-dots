## Desafío: Más puntos

Ahora vas a hacer el juego más difícil cuanto más tiempo lo juegue el jugador. Hará esto haciendo que los puntos aparezcan más y más rápido con el tiempo.

\--- tarea \--- Crea una nueva `variable`{: class = "block3variables"} llamada 'retraso'.

![Sprite de escenario](images/stage-sprite.png) \--- /task \---

\--- task \--- Vaya al área de Scripts del escenario y cree un nuevo script que establezca la variable `delay`{: class = "block3variables"} en `8` y luego reduzca lentamente el valor de `delay`{: class = "block3variables"} mientras se ejecuta el juego.

![Sprite de escenario](images/stage-sprite.png)

```blocks3
    cuando se hace clic en el indicador
    establezca [retraso v] a (8)
    repita hasta < (retraso) = (2)>
        espere (10) segundos
        cambie [retraso v] por (-0.5)
    fin
```

\--- /task \---

¡Observe que este código es muy similar al código que usaría para crear un temporizador de cuenta regresiva!

A continuación, utilice la variable `delay`{: class = "block3variables"} en los scripts de código de los sprites 'rojo', 'amarillo' y 'azul'.

\--- tarea \--- Elimina el bloque de código que hace que el juego espere un número aleatorio de segundos entre los clones de sprite de puntos. Vuelva a colocar el bloque que ha sacado con su nuevo `retardo`{: class = "block3variables"} variables:

![screenshot](images/all-dots.png)

```blocks3
<br />- esperar (elegir aleatoriamente (5) a (10)) segundos
    esperar (retraso :: variables) segundos
```

Haga esto para los tres sprites de puntos.

\--- /task \---

\--- tarea \--- Prueba el juego y comprueba si los puntos comienzan a aparecer más rápidamente a medida que avanza el juego.

+ ¿Esto funciona para los tres puntos de colores?
+ ¿Puedes ver que el valor del `retardo`{: class = "block3variables"} disminuye? \--- /task \---