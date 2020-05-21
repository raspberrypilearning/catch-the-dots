## Crear un controlador

Comienza creando un controlador que el jugador utilizará para atrapar los puntos.

\--- task \---

Abre el proyecto inicial de Scratch 'Captura los puntos'.

**En línea:** abre el proyecto inicial en [rpf.io/dots-on](http://rpf.io/dots-on){:target="_blank"}.

Si tienes una cuenta de Scratch puedes hacer una copia haciendo clic en **Remix**.

**Sin conexión:** descarga el proyecto inicial desde [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go) y luego ábrelo con el editor de Scratch sin conexión.

Si necesitas descargar e instalar el editor de Scratch offline, puedes encontrarlo en [ rpf.io/scratchoff ](http://rpf.io/scratchoff).

\--- /task \---

Debes ver el objeto llamado controlador:

![captura de pantalla](images/dots-controller.png)

\--- task \---

Agrega código al objeto del controlador para hacer que el objeto gire a la derecha si el jugador presiona la tecla de flecha derecha:

![Objeto controlador](images/controller-sprite.png)

```blocks3
    al hacer clic en la bandera
    para siempre
        si <key (right arrow v) pressed?> luego
            gira a la derecha (3) grados
        end
    end
```

\--- /task \---

\--- task \---

Prueba tu código. El controlador debe girar a la derecha cuando presionas la flecha hacia la derecha.

\--- /task \---

\--- task \---

Añade código al objeto controlador para hacer que el objeto gire a la izquierda si el jugador presiona la tecla de flecha izquierda.

![Objeto controlador](images/controller-sprite.png)

\--- hints \---

\--- hint \---

Encuentra el código que verifica si la flecha hacia la derecha ha sido presionada y hace que el objeto gire hacia la derecha. ¿Puedes agregar una copia de este código y cambiarla de manera que verifique si la flecha hacia la izquierda ha sido presionada y haga que el objeto gire a la izquierda?

\--- /hint \---

\--- hint \---

Aquí están los bloques que necesitas:

```blocks3
<key (space v) pressed?>

girar a la izquierda (15) grados

si <> entonces

final
```

\--- /hint \---

\--- hint \---

Así es como debe verse tu código:

```blocks3
    al hacer clic en bandera
    para siempre
        si <key (right arrow v) pressed?> luego
            gira a la derecha (3) grados
        end

+ si <key (left arrow v) pressed?> entonces
            gira a la izquierda (3) grados
        end
    end
```

\--- /hint \---

\--- /hints \---

\--- /task \---