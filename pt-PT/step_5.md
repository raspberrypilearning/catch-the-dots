## Aumentar a dificuldade

Agora vais tornar o jogo mais difícil à medida que o jogador o for jogando. Fazes isso fazendo com que os pontos apareçam mais rápido à medida que o tempo passa.

\--- task \--- Cria uma nova `variável`{:class="block3variables"} chamada 'atraso'.

![Stage sprite](images/stage-sprite.png) \--- /task \---

\--- task \--- Vai para a área dos Guiões do Palco e cria um novo guiāo que altera a variável `atraso`{:class="block3variables"} para `8` e depois lentamente reduz o valor de `atraso`{:class="block3variables"} enquanto o jogo corre.

![Stage sprite](images/stage-sprite.png)

```blocks3
    when flag clicked
    set [delay v] to (8)
    repeat until < (delay) = (2)>
        wait (10) seconds
        change [delay v] by (-0.5)
    end
```

\--- /task \---

Nota que este código é muito parecido com o código que usarias para fazer um temporizador de contagem regressiva!

Next, use the `delay`{:class="block3variables"} variable in the code scripts of the 'red', 'yellow', and 'blue' sprites.

\--- task \--- Remove the code block that makes the game wait a random number of seconds between making the dot sprite clones. Replace the block you've removed with your new `delay`{:class="block3variables"} variable:

![screenshot](images/all-dots.png)

```blocks3
<br />-   wait (pick random (5) to (10)) secs
    wait (delay :: variables) secs
```

Do this for all three dot sprites.

\--- /task \---

\--- task \--- Test the game, and check whether the dots begin to appear more quickly as the game goes on.

+ Does this work for all three coloured dots?
+ Can you see that the value of the `delay`{:class="block3variables"} variable decreases? \--- /task \---