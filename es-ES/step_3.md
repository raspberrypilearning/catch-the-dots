## Gana puntos o pierde vidas

Ahora vas a agregar algunos puntos que el jugador necesita recoger.

\--- task \---

Crea un nuevo objeto llamado 'rojo'. Este objeto debe ser un pequeño punto rojo.

![Objeto punto rojo](images/dots-red.png)

\--- /task \---

\--- task \---

Agrega este código a tu objeto 'rojo' para crear un nuevo clon del objeto cada pocos segundos:

![Objeto punto rojo](images/red-sprite.png)

```blocks3
    al hacer clic en la bandera
    ocultar
    esperar (2) segundos
    para siempre
        crear clon de (myself v)
        esperar (número al azar (5) a (10)) segundos
    final
```

\--- /task \---

Si ahora haces clic en la bandera verde, parece que nada está sucediendo. Esto se debe a que todos los objetos clonados están ocultos y aparecen en el mismo lugar.

Vas a agregar código para hacer que cada nuevo clon aparezca en una de las cuatro esquinas del escenario.

![captura de pantalla](images/dots-start.png)

\--- task \---

Crea una nueva lista llamada `posiciones de inicio`{:class="block3variables"}, haz clic en el icono `(+)` de la lista para añadir los valores `-180`{:class="block3variables"} y `180`{:class="block3variables"}.

![Objeto punto rojo](images/red-sprite.png)

![Lista de 180 y -180](images/dots-list.png)

[[[generic-scratch3-make-list]]]

Luego puedes ocultar la lista desmarcando este cuadro:

![Oculta la lista](images/hide-list.png)

\--- /task \---

Observa que la coordenada para cada esquina del escenario es una combinación de `180` y `-180`. Esto significa que puedes usar la lista para elegir una esquina del escenario al azar.

\--- task \---

Agrega este código al objeto 'punto' para hacer que cada nuevo clon aparezca en una esquina aleatoria y luego se mueva lentamente hacia el objeto controlador.

![Objeto punto rojo](images/red-sprite.png)

```blocks3
    al comenzar como clon
  ir a x: (elemento (número aleatorio entre (1) y (2)) de [start positions v]) y: (elemento (número aleatorio entre (1) y (2)) de [start positions v])
  apuntar hacia (controlador v)
  mostrar
  repetir hasta que <touching (controller v)?> 
    mover (1) pasos
  end
```

\--- /task \---

Este nuevo código elige `-180` o `180` para las posiciones x e y, significa que cada clon del objeto 'punto' comienza en una esquina del escenario.

\--- task \---

Prueba tu proyecto. Deberías ver puntos rojos que aparecen en las esquinas del escenario y se mueven lentamente hacia el controlador.

![captura de pantalla](images/dots-red-test.png)

\--- /task \---

\--- task \---

Crea dos nuevas variables llamadas `vidas`{:class="block3variables"} y `puntos`{:class="block3variables"}.

![Objeto punto rojo](images/red-sprite.png)

\--- /task \---

\--- task \---

Agrega código a tu escenario para dar a `vidas`{: clase = "block3variables"} el valor `3` y dar a `puntos`{: clase = "block3variables"} el valor `0` al inicio del juego. ![Objeto escenario](images/stage-sprite.png)

```blocks3
al hacer clic en la bandera
dar a [vidas v] el valor (3)
dar a [puntos v] el valor (0)
```

\--- /task \---

\--- task \---

Agrega este código al final de la secuencia de comandos del escenario para que el juego termine cuando el jugador pierde la última vida:

![Objeto escenario](images/stage-sprite.png)

```blocks3
    esperar hasta que <(vidas :: variables) < [1]>
    detener [todos v]
```

\--- /task \---

El jugador debe ganar puntos por atrapar puntos, y perder vidas por no haber conseguido puntos. Un punto solo puede capturarse haciendo coincidir el color del controlador con el color del punto.

\--- task \---

Vuelve a la zona de código del objeto 'rojo' para agregar algunos bloques al final del conjunto de bloques que comienza con: `cuando comienzo como un clon`{:class = "block3control"}.

Primero, haz que el clon rojo se `mueva 5 pasos`{:class = "block3motion"} para que se superponga al controlador.

Luego agrega el código para sumar `1` a `puntos`{: clase = "block3variables"} si el color del clon coincide con el color del controlador cuando se tocan, o para restar `1` a `vidas`{:class = "block3variables"} si sus colores no coinciden.

[[[generic-scratch3-sound-from-library]]]

![Objeto punto rojo](images/red-sprite.png)

```blocks3
    mover (5) pasos
si <touching color [#FF0000]?> entonces 
  sumar a [puntos v] (1)
  tocar sonido (pop v) hasta que termine
si no 
  sumar a [vidas v] (-1)
  tocar sonido (Laser1 v) hasta que termine
fin
eliminar este clon
```

\--- /task \---

\--- task \---

Prueba tu juego para asegurarte de que:

1. Pierdes una vida si no haces coincidir un punto con el color correcto
2. Aumentas tus puntos en 1 si lo haces coincidir

\--- /task \---