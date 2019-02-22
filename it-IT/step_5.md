## Aumentare la difficoltà

Ora renderai il gioco più difficile più a lungo il giocatore lo gioca. Lo farai facendo apparire i punti sempre più velocemente nel tempo.

\--- task \--- Crea una nuova variabile ``{: class = "block3variables"} chiamata "delay".

![Stage sprite](images/stage-sprite.png) \--- /compito \---

\--- task \--- Passare all'area Scripts dello stage e creare un nuovo script che imposta la variabile `delay`{: class = "block3variables"} su `8` e quindi riduce lentamente il valore di `delay`{: class = "block3variables"} durante il gioco.

![Stage sprite](images/stage-sprite.png)

```blocks3
    quando il flag ha cliccato
    impostato [delay v] to (8)
    repeat fino a < (delay) = (2)>
        wait (10) secondi
        change [delay v] di (-0.5)
    end
```

\--- /compito \---

Nota che questo codice è molto simile al codice che useresti per creare un timer per il conto alla rovescia!

Successivamente, usa la variabile `delay`{: class = "block3variables"} negli script di codice degli sprite "rosso", "giallo" e "blu".

\--- task \--- Rimuovi il blocco di codice che fa attendere al gioco un numero casuale di secondi tra la creazione dei cloni di sprite di punti. Sostituisci il blocco che hai rimosso con la nuova variabile `ritardo`{: class = "block3variables"}:

![immagine dello schermo](images/all-dots.png)

```blocks3
<br />- wait (seleziona casuale (5) a (10)) sec
    wait (delay :: variables) secs
```

Fallo per tutti e tre i punti sprites.

\--- /compito \---

\--- task \--- Prova il gioco e controlla se i punti iniziano ad apparire più velocemente mentre il gioco va avanti.

+ Funziona per tutti e tre i punti colorati?
+ Riesci a vedere che il valore della variabile `delay`{: class = "block3variables"} diminuisce? \--- /compito \---