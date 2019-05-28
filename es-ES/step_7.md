## Reto: Crear más bloques

Vas a guardar la puntuación más alta del juego, para que los jugadores puedan ver qué tan bien lo están haciendo.

\--- tarea \--- Crea una nueva variable llamada `puntuación alta`{: class = "block3variables"}.

![Sprite de escenario](images/stage-sprite.png)

\--- /task \---

\--- tarea \--- Selecciona el escenario. Haga clic en 'Mis bloques' y cree un nuevo bloque personalizado llamado `ver puntuación alta`{: class = "block3myblocks"}.

![Sprite de escenario](images/stage-sprite.png) ![captura de pantalla](images/dots-custom-1.png)

\--- /task \---

\--- tarea \--- Agregue código a su bloque personalizado para que el bloque verifique si el valor actual de `puntuación`{: clase = "block3variables"} en un valor mayor que el valor de `puntuación alta`{: clase = variable "block3variables"}, y luego almacena el valor de `score`{: class = "block3variables"} como el nuevo valor de `high score`{: class = "block3variables"}.

![Sprite de escenario](images/stage-sprite.png)

```blocks3
    definir cheque puntuación alta
    si <(puntuación :: variables) > (puntuación alta)> luego
        series [puntuación alta v] a (puntuación :: variables)
    final
```

\--- /task \---

\--- tarea \--- Agregue su nuevo bloque personalizado a la secuencia de comandos de Stage antes del final de la secuencia de comandos.

![Sprite de escenario](images/stage-sprite.png)

```blocks3
cuando se hace clic en el indicador
establecer [vidas v] a (3)
establecer [puntuación v] a (0)
esperar hasta <(vidas) < (1)>

+ verificar puntuación alta :: costumbre
detener [todas v]
```

\--- /task \---

\--- task \---

Juegue su juego dos veces para comprobar si su puntuación se guarda correctamente como la puntuación alta ``{: class = "block3variables"}.

\--- /task \---