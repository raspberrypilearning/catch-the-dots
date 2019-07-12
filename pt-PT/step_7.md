## Melhor pontuação

Vais guardar a melhor pontuaçāo do jogo, de modo que os jogadores possam avaliar o seu desempenho.

\--- task \--- Cria uma nova variável chamada `melhor pontuaçāo`{:class="block3variables"}.

![Actor palco](images/stage-sprite.png)

\--- /task \---

\--- task \--- Seleciona o Palco. Clica em 'Os meus blocos' e cria um novo bloco personalizado chamado `cVerificar melhor pontuaçāo`{:class="block3myblocks"}.

![Actor palco](images/stage-sprite.png) ![captura de ecrã](images/dots-custom-1.png)

\--- /task \---

\--- task \--- Adiciona código ao teu novo bloco personalizado para que ele verifique se o valor actual de `pontuaçāo`{:class="block3variables"} é maior que o valor da variável `melhor pontuaçāo`{:class="block3variables"}, e depois guarda o valor de `pontuaçāo`{:class="block3variables"} como novo valor de `melhor pontuaçāo`{:class="block3variables"}.

![Actor palco](images/stage-sprite.png)

```blocks3
    define check high score
    if <(score :: variables) > (high score)> then
        set [high score v] to (score :: variables)
    end
```

\--- /task \---

\--- task \--- Add your new custom block to the Stage script before the end of the script.

![Actor palco](images/stage-sprite.png)

```blocks3
when flag clicked
set [lives v] to (3)
set [score v] to (0)
wait until <(lives) < (1)>

+ check high score :: custom
stop [all v]
```

\--- /task \---

\--- task \---

Joga o teu jogo duas vezes para verificar se a tua pontuaçāo é guardada corretamente como a `melhor pontuaçāo`{:class="block3variables"}.

\--- /task \---