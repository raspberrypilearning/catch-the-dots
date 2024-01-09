## Più puntini

\--- task \---

Duplica due volte il tuo sprite "rosso" e dai un nome ai due nuovi sprite "giallo" e "blu".

![screenshot](images/dots-more-dots.png)

\--- /task \---

\--- task \---

Cambia il costume di ogni nuovo sprite in modo che sia del colore corretto: lo sprite "giallo" dovrebbe essere giallo e lo sprite "blu" dovrebbe essere blu.

\--- /task \---

\--- task \---

Cambia il codice di ogni sprite in modo che il giocatore debba abbinare il clone puntino al colore corretto sul controller per ottenere punti.

![screenshot](images/dots-all-test.png)

\--- hints \---

\--- hint \---

Questo è il codice che devi trovare e modificare per entrambe i nuovi sprite:

![screenshot](images/dots-more-dots.png)

```blocks3
    if <touching color [#FF0000]?> then
        change [score v] by (1)
        play sound (pop v)
        ...
    end
```

\--- /hint \---

\--- hint \---

Ecco come è necessario modificare il codice per lo sprite giallo:

```blocks3
    if <touching color [#FFFF00]? :: +> then
        change [score v] by (1)
        play sound (pop v)
    end
```

Ecco come è necessario modificare il codice per lo sprite blu:

```blocks3
    if <touching color [#0000FF]? :: +> then
        change [score v] by (1)
        play sound (pop v)
    end
```

\--- /hint \---

\--- /hints \---

\--- /task \---

Se giochi ora, noterai che i punti a volte vengono creati uno sopra l'altro.

\--- task \---

Cambia il codice dello sprite 'giallo' in modo che attenda quattro secondi, prima di apparire, dopo che si fa clic sulla bandiera.

![Puntino giallo](images/yellow-sprite.png)

```blocks3
    when flag clicked
    hide
+   wait (4) seconds
```

![Puntino blu](images/blue-sprite.png)

Ora cambia il codice dello sprite "blu" in modo che attenda 6 secondi, prima di apparire, dopo che si fa clic sulla bandiera.

\--- /task \---