## Criar um controlador

Começa por criar um controlador que o jogador vai usar para apanhar os pontos.

Abre o projeto Scratch inicial 'Apanha os pontos'.

**Online:** abre um novo projeto online Scratch em [rpf.io/dots-on](http://rpf.io/dots-on){:target="_blank"}.

Se tiveres uma 'conta Scratch podes fazer uma cópia ao clicares **Remix**.

**Offline:** descarrega o projeto inicial de [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go), e abre-o no editor Scratch offline.

Se precisares de descarregar e instalar o editor offline do Scratch, podes encontrá-lo em [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /task \---

Deves ver um actor 'controlador':

![screenshot](images/dots-controller.png)

\--- task \--- Adiciona código ao actor controlador para o fazer rodar para a direita se o jogador premir a tecla 'seta para a direita':

![Controller sprite](images/controller-sprite.png)

```blocks3
    when flag clicked
    forever
        if <key (right arrow v) pressed?> then
            turn right (3) degrees
        end
    end
```

\--- /task \---

\--- task \--- Test your code. The controller should spin to the right when you press the right arrow key. \--- /task \---

\--- task \--- Add code to the controller sprite to make the sprite turn left if the player presses the left arrow key.

![Controller sprite](images/controller-sprite.png)

\--- hints \--- \--- hint \---

Find the code that checks whether the right arrow key is pressed and makes the sprite turn right. Can you add a copy of this code, and change the copy so it checks whether the left arrow key is pressed and makes the sprite turn left?

\--- /hint \--- \--- hint \--- Here are the blocks you need:

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

\--- /hint \--- \--- hint \--- Here is what your code should look like:

```blocks3
    when flag clicked
    forever
        if <key (right arrow v) pressed?> then
            turn right (3) degrees
        end

+       if <key (left arrow v) pressed?> then
            turn left(3) degrees
        end
    end
```

\--- /hint \--- \--- /hints \--- \--- /task \---