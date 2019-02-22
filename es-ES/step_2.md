## Crear un controlador

Comience creando un controlador que el jugador utilizará para recoger puntos.

\--- tarea \--- Abra el proyecto de arranque de Scratch 'Catch the dots'.

**En línea:** abra el proyecto de inicio en [rpf.io/dots-on](http://rpf.io/dots-on){: target = "_ blank"}. Si tiene una cuenta de Scratch, puede hacer clic en **Remix** en la esquina superior derecha para guardar una copia del proyecto.

**Desconectado:** de descargar el proyecto inicial de [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go), y luego abrirlo en el editor de Scratch en línea.

Si necesita descargar e instalar el editor de Scratch offline, puede encontrarlo en [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- / tarea \---

Deberías ver un controlador sprite:

![captura de pantalla](images/dots-controller.png)

\--- tarea \--- Agregue algo de código al controlador sprite para que gire a la derecha si el jugador presiona la tecla de flecha derecha:

![Controlador sprite](images/controller-sprite.png)

```blocks3
    cuando la bandera hace clic en
    para siempre
        si <key (right arrow v) pressed?> luego
            gira a la derecha (3) grados
        final
    final
```

\--- / tarea \---

\--- tarea \--- Pon a prueba tu código. El controlador debe girar hacia la derecha cuando presiona la tecla de flecha derecha. \--- / tarea \---

\--- tarea \--- Agregue código al sprite del controlador para hacer que el sprite gire a la izquierda si el jugador presiona la tecla de flecha izquierda.

![Controlador sprite](images/controller-sprite.png)

\--- consejos \--- \--- consejo \---

Encuentre el código que verifica si se presiona la tecla de flecha derecha y hace que el sprite gire a la derecha. ¿Puede agregar una copia de este código y cambiar la copia para que compruebe si se presiona la tecla de flecha izquierda y hace que el sprite gire a la izquierda?

\--- / hint \--- \--- hint \--- Aquí están los bloques que necesitas:

```blocks3
<key (space v) pressed?>

gire a la izquierda (15) grados

si <> luego

final
```

\--- / hint \--- \--- hint \--- Aquí está el aspecto que debería tener tu código:

```blocks3
    cuando la bandera hace clic en
    para siempre
        si <key (right arrow v) pressed?> luego
            gira a la derecha (3) grados
        termina

+ si <key (left arrow v) pressed?> luego
            gira a la izquierda (3) grados
        final
    final
```

\--- / hint \--- \--- / hints \--- \--- / task \---