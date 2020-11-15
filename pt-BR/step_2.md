## Crie o controle

Comece a criar um controlador que o jogador vai usar para apanhar os pontos.

\--- task \---

Abra o projeto Scratch inicial 'Capture Bolinhas'.

**Online:** Abra o projeto inicial em [ rpf.io/dots-on ](http://rpf.io/dots-on){: target="_ blank"}.

Se você tiver uma conta Scratch, você pode fazer uma cópia clicando em **Remix**.

**Offline:** baixe o projeto inicial de [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go), e depois abra-o no editor Scratch offline.

Se você precisar baixar e instalar o editor offline do Scratch, você pode encontrá-lo em [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /task \---

Você deve ver uma imagem do ator do controlador:

![captura de tela](images/dots-controller.png)

\--- task \---

Adicione código ao ator do controlador para fazê-lo girar para a direita se o jogador pressionar a tecla de seta para a direita:

![Ator Controle](images/controller-sprite.png)

```blocks3
    when flag clicked
    forever
        if <key (right arrow v) pressed?> then
            turn right (3) degrees
        end
    end
```

\--- /task \---

\--- task \---

Teste seu código. O controle deve girar para a direita quando você pressionar a tecla de seta para a direita.

\--- /task \---

\--- task \---

Adicione código ao ator Controle para faze-lo girar para a esquerda se o jogador pressionar a tecla de seta para a esquerda.

![Ator Controle](images/controller-sprite.png)

\--- hints \---

\--- hint \---

Find the code that checks whether the right arrow key is pressed and makes the sprite turn right. Can you add a copy of this code, and change the copy so it checks whether the left arrow key is pressed and makes the sprite turn left?

\--- /hint \---

\--- hint \---

Here are the blocks you need:

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

\--- /hint \---

\--- hint \---

Here is what your code should look like:

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

\--- /hint \---

\--- /hints \---

\--- /task \---