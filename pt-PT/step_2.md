## Criar um controlador

Começa por criar um controlador que o jogador vai usar para apanhar os pontos.

Abre o projeto Scratch inicial 'Apanha os pontos'.

**Online:** abre um novo projeto online Scratch em [rpf.io/dots-on](http://rpf.io/dots-on){:target="_blank"}.

Se tiveres uma 'conta Scratch podes fazer uma cópia ao clicares **Remix**.

**Offline:** descarrega o projeto inicial de [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go), e abre-o no editor Scratch offline.

Se precisares de descarregar e instalar o editor offline do Scratch, podes encontrá-lo em [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /task \---

Deves ver um actor 'controlador':

![screenshot](images/dots-controller.png)

\--- task \--- Adiciona código ao actor controlador para o fazer rodar para a direita se o jogador premir a tecla 'seta para a direita':

![Controller sprite](images/controller-sprite.png)

```blocks3
    quando alguem clicar na bandeira
    para sempre
        se <key (right arrow v) pressed?> entāo
            roda para a direita (3) graus
        termina
    termina
```

\--- /task \---

\--- task \--- Testa o teu código. O controlador deve rodar para a direita quando primes a 'seta para a direita'. \--- /task \---

\--- task \--- Adiciona código ao actor controlador para o fazer rodar para a esquerda se o jogador premir a tecla 'seta para a esquerda'.

![Controller sprite](images/controller-sprite.png)

\--- hints \--- \--- hint \---

Encontra o código que verifica se a a 'seta para a direita' ė premida e faz o actor rodar para a direita. Podes adicionar uma cópia deste código, e mudar a cópia de maneira a que verifique se a tecla 'seta para a esquerda' está premida e fazer o actor rodar para a esquerda?

\--- /hint \--- \--- hint \--- Aqui estão os blocos que precisas:

```blocks3
<key (space v) pressed?>

roda para a esquerda (15) degrees

se <> entāo

termina
```

\--- /hint \--- \--- hint \--- Aqui está como o teu código deve parecer:

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