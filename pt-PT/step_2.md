## Criar um controlador

Começa por criar um controlador que o jogador vai usar para apanhar os pontos.

Abre o projeto Scratch inicial 'Apanha os pontos'.

**Online:** abre o projeto inicial Scratch em [rpf.io/dots-on](http://rpf.io/dots-on){:target="_blank"}.

Se tiveres uma 'conta Scratch' podes fazer uma cópia ao clicares **Remix**.

**Offline:** descarrega o projeto inicial de [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go), e depois abre-o no editor Scratch offline.

Se precisares de descarregar e instalar o editor offline do Scratch, podes encontrá-lo em [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /task \---

Deves ver um actor 'controlador':

![captura de ecrã](images/dots-controller.png)

\--- task \--- Adiciona código ao actor 'controlador' para o fazer girar para a direita se o jogador premir a tecla 'seta para a direita':

![Actor controlador](images/controller-sprite.png)

```blocks3
    quando alguém clicar na bandeira
    para sempre
        se <key (right arrow v) pressed?> entāo
            gira para a direita (3) graus
        terminar
    terminar
```

\--- /task \---

\--- task \--- Testa o teu código. O 'controlador' deve girar para a direita quando primes a tecla 'seta para a direita'. \--- /task \---

\--- task \--- Adiciona código ao actor 'controlador' para o fazer rodar para a esquerda se o jogador premir a tecla 'seta para a esquerda'.

![Actor controlador](images/controller-sprite.png)

\--- hints \--- \--- hint \---

Encontra o código que verifica se a a 'seta para a direita' ė premida e faz o actor girar para a direita. Podes adicionar uma cópia deste código, e mudar a cópia de maneira a que verifique se a tecla 'seta para a esquerda' está premida e fazer o actor girar para a esquerda?

\--- /hint \--- \--- hint \--- Aqui estão os blocos que precisas:

```blocks3
<key (space v) pressed?>

roda para a esquerda (15) degrees

se <> entāo

termina
```

\--- /hint \--- \--- hint \--- Aqui está como o teu código deve parecer:

```blocks3
    quando alguém clicar na bandeira
    repete para sempre
        se <key (right arrow v) pressed?> entāo
            roda para a direita (3) graus
        terminar

+       se <key (left arrow v) pressed?> entāo
            roda para a esquerda (3) graus
        terminar
    terminar
```

\--- /hint \--- \--- /hints \--- \--- /task \---