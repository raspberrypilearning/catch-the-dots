## Más puntos

\--- tarea \--- Duplica el sprite de puntos 'rojo' dos veces y nombra a los dos nuevos sprites 'amarillo' y 'azul'.

![captura de pantalla](images/dots-more-dots.png) \--- / tarea \---

\--- tarea \--- Cambia el traje de cada nuevo sprite para que tenga el color correcto: el sprite 'amarillo' debe ser amarillo, y el sprite 'azul' debe ser azul. \--- / tarea \---

\--- tarea \--- Cambia el código de cada sprite para que el jugador tenga que hacer coincidir el clon de puntos con el color correcto en el controlador para obtener puntos.

![captura de pantalla](images/dots-all-test.png)

\--- consejos \--- \--- consejo \--- Este es el código que debes encontrar y modificar para los dos nuevos sprites:

![captura de pantalla](images/dots-more-dots.png)

```blocks3
    si <touching color [#FF0000]?> entonces
        cambia [puntuación v] por (1)
        sonido de reproducción (pop v)
...
    fin
```

\--- / hint \--- \--- hint \--- Así es como necesitas cambiar el código para el sprite amarillo:

```blocks3
    si <toca el color [# FFFF00]? :: +> luego
        cambia [puntuación v] por (1)
        reproducir sonido (pop v)
    final
```

Así es como necesitas cambiar el código para el sprite azul:

```blocks3
    si <toca el color [# 0000FF]? :: +> luego
        cambia [puntuación v] por (1)
        reproducir sonido (pop v)
    final
```

\--- / hint \--- \--- / hints \--- \--- / task \---

Si juegas ahora, puedes ver que los puntos a veces se crean uno encima del otro.

\--- tarea \--- Cambie el código para el sprite de punto 'amarillo' para que espere cuatro segundos después de hacer clic en la bandera antes de aparecer.

![Punto amarillo](images/yellow-sprite.png)

```blocks3
    cuando se hace clic en la bandera
    ocultar
+ esperar (4) segundos
```

![Punto azul](images/blue-sprite.png)

Luego, cambie el código para el punto sprite 'azul' para que espere 6 segundos después de hacer clic en la bandera antes de aparecer.

\--- / tarea \---