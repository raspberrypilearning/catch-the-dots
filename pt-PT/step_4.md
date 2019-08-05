## Mais 'pontos'

\--- task \--- Duplica o teu actor ponto 'vermelho' duas vezes, e nomeia os dois novos actores de 'amarelo' e 'azul'.

![captura de ecrã](images/dots-more-dots.png) \--- /task \---

\--- task \--- Muda o traje de cada actor para a cor correta: o actor 'amarelo' deve ser amarelo, e o 'azul' azul. \--- /task \---

\--- task \--- Muda a cor de cada actor de maneira a que o jogador tenha que acertar o 'ponto' clone com a cor correta no controlador para marcar pontos.

![captura de ecrã](images/dots-all-test.png)

\--- hints \--- \--- hint \--- Este é o código que precisas de encontrar e alterar para ambos os actores:

![captura de ecrã](images/dots-more-dots.png)

```blocks3
    se <estás a tocar na cor [#FF0000]> , então 
  adiciona a [score v] o valor (1)
  toca o som (pop v)
  . . ...
    end
```

\--- /hint \--- \--- hint \--- Aqui está como precisas de mudar o código para o actor amarelo:

```blocks3
    if &lt;touching color [#FFFF00]? se <estás a tocar na cor [#FFFF00]:: +>, então 
  adiciona a [score v] o valor (1)
  toca o som (pop v)
end
```

Assim é como precisas de mudar o código para o actor azul:

```blocks3
    se <estás a tocar na cor [#0000FF]? :: +>, então 
  adiciona a [score v] o valor (1)
  toca o som (pop v)
end
```

\--- /hint \--- \--- /hints \--- \--- /task \---

Se jogares o jogo agora, podes ver que ás vezes os pontos sāo criados um em cima do outro.

\--- task \--- Muda o código do actor 'amarelo' para que espere quatro segundos depois de a bandeira ser clicada antes de aparecer.

![Ponto amarelo](images/yellow-sprite.png)

```blocks3
    Quando alguém clicar na bandeira verde
    esconde-te
+    espera (4) s
```

![Ponto azul](images/blue-sprite.png)

Depois muda o código do actor 'azul' para que espere 6 segundos, depois de a bandeira ser clicada, antes de aparecer.

\--- /task \---