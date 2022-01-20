## Crear un controlador

Comienza creando un controlador que el jugador utilizará para atrapar los puntos.

--- task ---

Abre el proyecto inicial de Scratch 'Captura los puntos'.

**En línea:** abre el proyecto inicial en [scratch.mit.edu/projects/398085696](https://scratch.mit.edu/projects/398085696){:target="_blank"}.

Si tienes una cuenta de Scratch puedes hacer una copia haciendo clic en **Remix**.

**Sin conexión:** descarga el proyecto inicial desde [rpf.io/p/es-ES/catch-the-dots-go](https://rpf.io/p/es-ES/catch-the-dots-go) y luego ábrelo con el editor de Scratch sin conexión.

Si necesitas descargar e instalar el editor de Scratch offline, puedes encontrarlo en [rpf.io/scratchoff](https://rpf.io/scratchoff).

--- /task ---

Debes ver el objeto llamado controlador:

![captura de pantalla](images/dots-controller.png)

--- task ---

Agrega código al objeto del controlador para hacer que el objeto gire a la derecha si el jugador presiona la tecla de flecha derecha:

![Objeto controlador](images/controller-sprite.png)

```blocks3
    when flag clicked
	forever
		if <key (right arrow v) pressed?> then
			turn right (3) degrees
		end
	end
```

--- /task ---

--- task ---

Prueba tu código. El controlador debe girar a la derecha cuando presionas la flecha hacia la derecha.

--- /task ---

--- task ---

Añade código al objeto controlador para hacer que el objeto gire a la izquierda si el jugador presiona la tecla de flecha izquierda.

![Objeto controlador](images/controller-sprite.png)

--- hints ---


--- hint ---

Encuentra el código que verifica si la flecha hacia la derecha ha sido presionada y hace que el objeto gire hacia la derecha. ¿Puedes agregar una copia de este código y cambiarla de manera que verifique si la flecha hacia la izquierda ha sido presionada y haga que el objeto gire a la izquierda?

--- /hint ---

--- hint ---

Aquí están los bloques que necesitas:

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

--- /hint ---

--- hint ---

Así es como debe verse tu código:

```blocks3
    when flag clicked
	forever
		if <key (right arrow v) pressed?> then
			turn right (3) degrees
		end
+ 		if <key (left arrow v) pressed?> then
			turn left(3) degrees
		end
	end
```

--- /hint ---

--- /hints ---

--- /task ---
