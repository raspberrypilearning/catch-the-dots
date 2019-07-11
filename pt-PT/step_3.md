## Ganhar pontos ou perder vidas

Agora vais adicionar alguns pontos que o jogador precisa de apanhar.

\--- task \--- Cria um novo actor chamado 'vermelho'. Este actor deve ser um pequeno ponto vermelho.

![Red dot sprite](images/dots-red.png)

\--- /task \---

\--- task \--- Adiciona este guiāo ao teu actor 'vermelho' para criar um novo clone do actor a cada poucos segundos:

![Red dot sprite](images/red-sprite.png)

```blocks3
    quando alguém clicar na bandeira
    esconde-te
    espera (2) segundos
    repete para sempre
        cria um clone  (de mim mesmo v)
        espera (escolhe ao acaso entre (5) e (10)) segundos
    terminar
```

\--- /task \---

Se clicares na bandeira verde agora, vai parecer que nāo acontece nada. Isso é por todos os actores clonados estāo escondidos, e aparecem no mesmo sítio.

Vais adicionar código para que cada novo clone apareça num dos quatro cantos do Palco.

![screenshot](images/dots-start.png)

\--- task \--- Cria uma nova lista chamada `posições iniciais`{:class="block3variables"}, clica o icone `(+)` da lista para adicionar os valores `--180`{:class="block3variables"} e `180`{:class="block3variables"}.

![Red dot sprite](images/red-sprite.png)

![List of 180 and -180](images/dots-list.png)

[[[generic-scratch3-make-list]]]

Depois podes esconder a lista se deselecionares esta opçāo:

![Hide the list](images/hide-list.png) \--- /task \---

Nota que as coordenadas para cada canto do Palco sāo uma combinaçāo de `180` e `-180`. Isso significa que podes usar a lista para escolher um canto do Palco ao acaso.

\--- task \--- Adiciona este código ao actor 'ponto' para que cada novo clone do actor apareça num canto ao acaso e depois lentamente se mova na direçāo do actor controlador.

![Red dot sprite](images/red-sprite.png)

```blocks3
    quando fores criado como um clone
    vai para a posiçāo x: (item (escolher ao acaso entre (1) e (2)) de  [posições iniciais v]) y: (item (pick random (1) e (2)) de [posições iniciais v])
    aponta em direçāo a (roda controladora v)
    motra-te
    repete até <touching (controller v)?>
        avança (1) passo
    terminar
```

\--- /task \--- Este novo código escolhe ou `-180` ou `180`o para as posições x e y, o que significa que cada actor 'ponto' começa num canto do Palco.

\--- task \--- Testa o teu projeto. Deves ver pontos vermelhos a aparecer nos cantos do Palco e moverem-se na direçāo do controlador.

![screenshot](images/dots-red-test.png) \--- /task \---

\--- task \--- Cria duas novas variáveis chamadas `vidas`{:class="block3variables"} e `pontuaçāo`{:class="block3variables"}.

![Red dot sprite](images/red-sprite.png) \--- /task \---

\--- task \--- Adiciona código ao teu Palco para alterar a variável `vidas`{:class="block3variables"} para `3` e `pontuaçāo`{:class="block3variables"} para `0` no inicio do jogo. ![Stage sprite](images/stage-sprite.png)

```blocks3
quando alguém clicar na bandeira
altera [vidas v] para (3)
altera [pontuaçāo v] to (0)
```

\--- /task \---

\--- task \--- Adiciona este código ao fim do guiāo do Palco para acabar o jogo quando o jogador perder a última das vidas:

![Stage sprite](images/stage-sprite.png)

```blocks3
    espera até <(vidas :: variavéis) < [1]>
    pára [tudo v]
```

\--- /task \---

O jogador deve ganhar pontos por apanhar pontos. e deve perder vidas por falhar. Um 'ponto' só pode ser apanhado se a cor do controlador for a mesma do 'ponto'.

\--- task \--- Volta à área do guiāo do actor 'vermelho' para adicionar alguns blocos ao fim do guiāo `Quando fores criado como um clone`{:class="block3control"} do actor.

First, make the dot clone `move 5 steps`{:class="block3motion"} so that it overlaps the controller.

Then add code to either add `1` to `score`{:class="block3variables"} if the colour of the dot clone matches the colour of the controller when they touch, or to take `1` away from `lives`{:class="block3variables"} if their colours don't match.

[[[generic-scratch3-sound-from-library]]]

![Red dot sprite](images/red-sprite.png)

```blocks3
    move (5) steps
    if <touching color [#FF0000]?> then
        change [score v] by (1)
        play sound (pop v) until done
    else
        change [lives v] by (-1)
        play sound (Laser1 v) until done
    end
    delete this clone
```

\--- /task \---

\--- task \---

Test your game to make sure that:

1. You lose a life if you don’t match a dot with the correct colour
2. You score a point if you match a dot correctly

\--- /task \---