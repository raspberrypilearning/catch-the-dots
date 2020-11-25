## Melhor pontuação

Você vai salvar a melhor pontuação do jogo, para que os jogadores possam ver como estão se saindo.

--- task ---

Crie uma nova variável chamada `melhor pontuação`{:class="block3variables"}.

![Ator Palco](images/stage-sprite.png)

--- /task ---

--- task ---

Selecione o Palco. Clique em 'Meus blocos', e crie um novo bloco personalizado chamado `conferir melhor pontuação`{:class="block3myblocks"}.

![Ator Palco](images/stage-sprite.png)

![captura de tela](images/dots-custom-1.png)

--- /task ---

--- task ---

Adicione o código ao seu bloco personalizado para que o bloco verifique se o valor atual de `pontuação`{:class="block3variables"} é maior que o valor da variável `melhor pontuação`{:class="block3variables"}, e então armazena o valor de `pontuação`{:class="block3variables"} como o novo valor de `melhor pontuação`{:class="block3variables"}.

![Ator Palco](images/stage-sprite.png)

```blocks3
    define conferir melhor pontuação
    if <(pontuação :: variables) > (melhor pontuação)> then
        set [melhor pontuação v] to (pontuação :: variables)
    end
```

--- /task ---

--- task ---

Adicione seu novo bloco personalizado ao script do Palco, antes do final do script.

![Ator Palco](images/stage-sprite.png)

```blocks3
when flag clicked
set [vidas v] to (3)
set [pontuação v] to (0)
wait until <(vidas) < (1)>
+ conferir melhor pontuação :: custom
stop [all v]
```

--- /task ---

--- task ---

Jogue seu jogo duas vezes para verificar se a sua pontuação é guardada corretamente como a `melhor pontuação`{:class="block3variables"}.

--- /task ---