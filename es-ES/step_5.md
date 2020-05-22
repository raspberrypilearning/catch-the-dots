## Aumenta la dificultad

Ahora vas a hacer el juego más difícil cuanto más tiempo juegue el jugador. Harás esto haciendo que los puntos aparezcan más y más rápido con el tiempo.

\--- task \---

Crea una nueva `variable`{:class = "block3variables"} llamada 'retraso'.

![Objeto escenario](images/stage-sprite.png)

\--- /task \---

\--- task \---

Ve al área de código del escenario y crea un nuevo script que de a la variable `retraso`{: class = "block3variables"} el valor `8` y luego reduzca lentamente el valor de `retraso`{:class = "block3variables"} mientras se ejecuta el juego.

![Objeto escenario](images/stage-sprite.png)

```blocks3
    al hacer clic en la bandera
    establecer [retraso v] a (8)
    repetir hasta < (retraso) = (2)>
        esperar (10) segundos
        cambiar [retraso v] por (-0.5)
    fin
```

\--- /task \---

¡Observa que este código es muy similar al código que usarías para crear un temporizador de cuenta regresiva!

A continuación, utiliza la variable `retraso`{:class = "block3variables"} en el código de los objetos 'rojo', 'amarillo' y 'azul'.

\--- task \---

Elimina el bloque de código que hace que el juego espere un número aleatorio de segundos entre los clones de los puntos. Vuelve a colocar el bloque que has quitado con tu nueva variable 0>retraso</code>{:class= "block3variables"} variable:

![captura de pantalla](images/all-dots.png)

```blocks3
<br />-  esperar (número aleatorio entre (5) y (10)) segundos
    esperar (retraso :: variables) segundos
```

Haz esto para los tres objetos puntos.

\--- /task \---

\--- task \---

Prueba el juego y verifica que los puntos comiencen a aparecer más rápidamente a medida que avanza el juego.

+ ¿Funciona para los tres puntos de colores?
+ ¿Puedes ver que el valor del `retraso`{:class= "block3variables"} disminuye?

\--- /task \---