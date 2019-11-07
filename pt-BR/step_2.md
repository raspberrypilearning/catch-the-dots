## Criar um controlador

Comece a criar um controlador que o jogador vai usar para apanhar os pontos.

Abra o projeto Scratch inicial 'Apanha os pontos'.

**Online:** Abra o projeto inicial em [ rpf.io/dots-on ](http://rpf.io/dots-on){: target="_ blank"}.

Se você tiver uma conta do Scratch, pode fazer uma cópia clicando em ** Remix **.

**Offline:** descarregue o projeto inicial de [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go), e depois abre-o no editor Scratch offline.

Se você precisar baixar e instalar o editor do Scratch offline, você pode encontrá-lo em [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /task \---

Você deve ver uma imagem do controlador:

![screenshot](images/dots-controller.png)

\--- task \--- Adicione um código ao 'controlador' para o fazer girar para a direita se o jogador pressionar a tecla 'seta para a direita':

![Controller sprite](images/controller-sprite.png)

```blocks3
    quando clicar em ⚑
  sempre 
    se <key (right arrow v) pressed?> então 
      gire ↻ (3) graus
    end
  end
```

\--- /task \---

\--- task \--- Testa o teu código. O 'controlador' deve girar para a direita quando pressionar a tecla 'seta para a direita'. \--- /task \---

\--- task \--- Adicione um código ao 'controlador' para o fazer girar para a direita se o jogador pressionar a tecla 'seta para a direita'.

![Controller sprite](images/controller-sprite.png)

\--- hints \--- \--- hint \---

Encontre o código que verifica se a 'seta para a direita' ė pressionada e faz o sprite girar para a direita. Pode adicionar uma cópia deste código, e mudar a cópia de maneira a que verifique se a tecla 'seta para a esquerda' está premida e fazer o sprite girar para a esquerda?

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