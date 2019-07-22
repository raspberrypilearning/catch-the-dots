## Mais 'pontos'

\--- task \--- Duplica o teu actor ponto 'vermelho' duas vezes, e nomeia os dois novos actores de 'amarelo' e 'azul'.

![captura de ecrã](images/dots-more-dots.png) \--- /task \---

\--- task \--- Muda o traje de cada actor para a coe correta: o actor 'amarelo' deve ser amarelo, e o 'azul' azul. \--- /task \---

\--- task \--- Muda a cor de cada actor de maneira a que o jogador tenha que acertar o 'ponto' clone com a cor correta no controlador para marcar pontos.

![captura de ecrã](images/dots-all-test.png)

\--- hints \--- \--- hint \--- Este é o oódigo que precisas de encontrar e alterar para ambos os actores:

![captura de ecrã](images/dots-more-dots.png)

```blocks3
    se <touching color [#FF0000]?> entāo
        altera [pontuaçāo v] por (1)
        toca o som (pop v)
        ...
    terminar
```

\--- /hint \--- \--- hint \--- Aqui está como precisas de mudar o código para o actor amarelo:

```blocks3
    if <touching color [#FFFF00]? :: +> then
        change [score v] by (1)
        play sound (pop v)
    end
```

Assim é como precisas de mudar o código para o actor azul:

```blocks3
    if <touching color [#0000FF]? :: +> then
        change [score v] by (1)
        play sound (pop v)
    end
```

\--- /hint \--- \--- /hints \--- \--- /task \---

Se jogares o jogo agora, podes que ver ás vezes os pontos sāo criados um em cima do outro.

\--- task \--- Muda o código do actor 'amarelo' para que espere quatro segundos depois de a bandeira ser clicada antes de aparecer.

![Ponto amarelo](images/yellow-sprite.png)

```blocks3
    when flag clicked
    hide
+   wait (4) seconds
```

![Ponto azul](images/blue-sprite.png)

Depois muda o código do actor 'azul' para que espere 6 segundos depois de a bandeira ser clicada antes de aparecer.

\--- /task \---