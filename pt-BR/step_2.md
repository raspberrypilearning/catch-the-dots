## Crie o controle

Comece a criar um controlador que o jogador vai usar para apanhar os pontos.

\--- task \---

Abra o projeto Scratch inicial 'Capture Bolinhas'.

**Online:** open the starter project at [rpf.io/dots-on](https://rpf.io/dots-on){:target="_blank"}.

Se você tiver uma conta Scratch, você pode fazer uma cópia clicando em **Remix**.

**Offline:** download the starter project from [rpf.io/p/en/catch-the-dots-go](https://rpf.io/p/en/catch-the-dots-go), and then open it in the Scratch offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff).

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

Encontre o código que verifica se a tecla de seta para a direita está pressionada e faz o ator girar para a direita. Você pode adicionar uma cópia deste código e alterar a cópia para que ela verifique se a tecla de seta para a esquerda está pressionada e faz o ator girar para a esquerda?

\--- /hint \---

\--- hint \---

Aqui estão os blocos que você precisa:

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

\--- /hint \---

\--- hint \---

É assim que seu código deve parecer:

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