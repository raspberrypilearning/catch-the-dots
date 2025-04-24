## Aumentare la difficoltà

Ora renderai il gioco più difficile più a lungo il giocatore lo gioca. Lo farai facendo apparire i punti sempre più velocemente nel tempo.

\--- task \---

Crea una nuova `variabile`{:class="block3variables"} chiamata 'ritardo'.

![Sprite dello stage](images/stage-sprite.png)

\--- /task \---

\--- task \---

Vai nell'area degli script dello Stage e crea un nuovo script che imposti la variabile `ritardo`{:class="block3variables"} a `8` e poi riduca lentamente il valore di `ritardo`{:class="block3variables"} durante l'esecuzione del gioco.

![Sprite dello stage](images/stage-sprite.png)

```blocks3
    when flag clicked
    set [delay v] to (8)
    repeat until < (delay) = (2)>
        wait (10) seconds
        change [delay v] by (-0.5)
    end
```

\--- /task \---

Nota che questo codice è molto simile al codice che useresti per creare un conto alla rovescia!

In seguito, usa la variabile `ritardo`{:class="block3variables"} negli script di codice degli sprite 'red', 'giallo' e 'blu'.

\--- task \---

Rimuovi il blocco di codice che fa aspettare il gioco un numero casuale di secondi tra la realizzazione di un clone dello sprite puntino e l'altro. Sostituisci il blocco che hai rimosso con la nuova variabile `ritardo`{:class="block3variables"}:

![screenshot](images/all-dots.png)

```blocks3
<br />-   wait (pick random (5) to (10)) secs
    wait (delay :: variables) secs
```

Fai questo per tutti e tre gli sprite.

\--- /task \---

\--- task \---

Prova il gioco e controlla se i punti cominciano ad apparire più velocemente mentre il gioco procede.

+ Funziona così per tutti e tre i puntini colorati?
+ Riesci a vedere che il valore della variabile `ritardo`{:class="block3variables"} diminuisce?

\--- /task \---