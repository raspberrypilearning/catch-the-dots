## Aumente a dificuldade

Agora você vai tornar o jogo mais difícil quanto mais tempo o jogador jogar. Você vai fazer isso fazendo com que as bolinhas apareçam mais rápido à medida que o tempo passa.

\--- task \---

Crie uma nova `variável`{:class="block3variables"} chamada 'atraso'.

![Ator Palco](images/stage-sprite.png)

\--- /task \---

\--- task \---

Vá para a área de scripts do Palco e crie um novo script que defina a variável `atraso`{:class="block3variables"} para `8` e então reduza lentamente o valor de `atraso`{:class="block3variables"} enquanto o jogo é executado.

![Ator Palco](images/stage-sprite.png)

```blocks3
    when flag clicked
    set [delay v] to (8)
    repeat until < (delay) = (2)>
        wait (10) seconds
        change [delay v] by (-0.5)
    end
```

\--- /task \---

Note que este código é muito parecido com o código que você usaria para fazer um temporizador de contagem regressiva!

Em seguida, use a variável `atraso`{:class="block3variables"} nos códigos dos atores das bolinhas 'vermelho', 'amarelo' e 'azul'.

\--- task \---

Remova o bloco de código que faz o jogo esperar um número aleatório de segundos entre a criação de clones das bolinhas. Substitua o bloco que você removeu com sua nova variável `atraso`{:class="block3variables"}:

![captura de tela](images/all-dots.png)

```blocks3
<br />-   wait (pick random (5) to (10)) secs
    wait (delay :: variables) secs
```

Faça isso para todos os três atores das bolinhas.

\--- /task \---

\--- task \---

Teste o jogo e verifique se as bolinhas começam a aparecer mais rapidamente à medida que o jogo avança.

+ Isto funciona com todas as três bolinhas coloridas?
+ Você consegue ver que o valor da variável `atraso`{:class="block3variables"} diminui?

\--- /task \---