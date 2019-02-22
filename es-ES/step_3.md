## Gana puntos o pierde vidas

Ahora vas a agregar algunos puntos que el jugador necesita recoger.

\--- tarea \--- Crea un nuevo sprite llamado 'rojo'. Este sprite debe ser un pequeño punto rojo.

![Sprite de punto rojo](images/dots-red.png)

\--- / tarea \---

\--- tarea \--- Agregue este script a su sprite 'rojo' para crear un nuevo clon del sprite cada pocos segundos:

![Sprite de punto rojo](images/red-sprite.png)

```blocks3
    cuando se hace clic en el indicador
    ocultar
    esperar (2) segundos
    para siempre
        crear un clon de (yo v)
        esperar (elegir al azar (5) a (10)) segundos
    fin
```

\--- / tarea \---

Si hace clic en la bandera verde ahora, parece que nada está sucediendo. Esto se debe a que todos los sprites clonados están ocultos y aparecen en el mismo lugar.

Va a agregar código para hacer que cada nuevo clon aparezca en una de las cuatro esquinas del escenario.

![captura de pantalla](images/dots-start.png)

\--- tarea \--- Crea una nueva lista llamada `posiciones de inicio`{: class = "block3variables"}, haz clic en el icono `(+)` la lista para agregar los valores `-180`{: class = "block3variables" } y `180`{: class = "block3variables"}.

![Sprite de punto rojo](images/red-sprite.png)

![Lista de 180 y -180](images/dots-list.png)

[[[generic-scratch3-make-list]]]

Luego puede ocultar la lista deseleccionando este cuadro:

![Ocultar la lista](images/hide-list.png) \--- / tarea \---

Observe que la coordenada para cada esquina del escenario es una combinación de `180` y `-180`. Esto significa que puede usar la lista para elegir un rincón del escenario al azar.

\--- tarea \--- Agregue este código al sprite 'punto' para hacer que cada nuevo clon de sprite aparezca en una esquina aleatoria y luego muévase lentamente hacia el sprite controlador.

![Sprite de punto rojo](images/red-sprite.png)

```blocks3
    cuando comience como un clon
    vaya a x: (elemento (selección aleatoria (1) a (2)) de [posiciones iniciales v]) y: (elemento (selección aleatoria (1) a (2)) de [posiciones iniciales v])
    punto hacia (controlador v)
    muestra
    repetición hasta que <touching (controller v)?>
        mueva (1) pasos
    final
```

\--- / task \--- Este nuevo código elige `-180` o `180` para las posiciones x e y, lo que significa que cada clon de sprite 'punto' comienza en una esquina del escenario.

\--- tarea \--- Pon a prueba tu proyecto. Debería ver aparecer puntos rojos en las esquinas del escenario y moverse lentamente hacia el controlador.

![captura de pantalla](images/dots-red-test.png) \--- / tarea \---

\--- tarea \--- Crea dos nuevas variables llamadas `vidas`{: clase = "block3variables"} y `puntuación`{: clase = "block3variables"}.

![Sprite de punto rojo](images/red-sprite.png) \--- / tarea \---

\--- tarea \--- Agregue código a su escenario para establecer la variable `vidas`{: clase = "block3variables"} en `3` y las `puntuaciones`{: clase = "block3variables"} en `0` at El inicio del juego. ![Sprite de escenario](images/stage-sprite.png)

```blocks3
cuando la bandera hace clic en
establece [vidas v] en (3)
establece [puntuación v] en (0)
```

\--- / tarea \---

\--- tarea \--- Agrega este código al final de la secuencia de comandos del escenario para que el juego termine cuando el jugador pierda la última vida:

![Sprite de escenario](images/stage-sprite.png)

```blocks3
    esperar hasta <(vidas :: variables) < [1]>
    detener [todos v]
```

\--- / tarea \---

El jugador debe ganar puntos por atrapar puntos, y debe perder vidas por no poder atrapar puntos. Un punto solo puede capturarse haciendo coincidir el color del controlador con el color del punto.

\--- \--- tarea Volver a la zona 'roja' del Objeto de puntos de secuencias de comandos para agregar algunos bloques de código al final del sprite de `cuando comienzo como un clon`{: class = "block3control"} guión.

Primero, haga que el punto clone `mueva 5 pasos`{: class = "block3motion"} para que se superponga al controlador.

Luego agregue el código para agregar `1` a `puntuación`{: clase = "block3variables"} si el color del clon de puntos coincide con el color del controlador cuando se tocan, o para quitar `1` de `vidas`{ : class = "block3variables"} si sus colores no coinciden.

[[[generic-scratch3-sound-from-library]]]

![Sprite de punto rojo](images/red-sprite.png)

```blocks3
    mueva (5) los pasos
    si <touching color [#FF0000]?> luego
        cambia [puntuación v] por (1)
        reproduce el sonido (pop v) hasta que termine
    más
        cambia [vidas v] por (-1)
        reproduce el sonido (Laser1 v) hasta que termine
    final
    borrar este clon
```

\--- / tarea \---

\--- tarea \---

Pruebe su juego para asegurarse de que pierde una vida si no hace coincidir un punto con el color correcto, y de que obtiene un punto si coincide con un punto correctamente.

\--- / tarea \---