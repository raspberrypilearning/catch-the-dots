## Punteggio alto

Stai per salvare il punteggio più alto del gioco, in modo che i giocatori possano vedere quanto stanno facendo bene.

\--- task \--- Crea una nuova variabile chiamata `high score`{: class = "block3variables"}.

![Stage sprite](images/stage-sprite.png)

\--- /compito \---

\--- task \--- Seleziona lo stage. Clicca su "I miei blocchi" e crea un nuovo blocco personalizzato chiamato `controlla il punteggio più alto`{: class = "block3myblocks"}.

![Stage sprite](images/stage-sprite.png) ![immagine dello schermo](images/dots-custom-1.png)

\--- /compito \---

\--- task \--- Aggiungi il codice al tuo blocco personalizzato in modo che il blocco controlli se il valore corrente di `punteggio`{: class = "block3variables"} in più del valore del punteggio massimo ``{: class = variabile "block3variables"}, quindi memorizza il valore di `score`{: class = "block3variables"} come nuovo valore di `high score`{: class = "block3variables"}.

![Stage sprite](images/stage-sprite.png)

```blocks3
    define check punteggio alto
    se <(punteggio :: variabili) > (punteggio alto)> poi
        set [punteggio alto v] a (punteggio :: variabili)
    fine
```

\--- /compito \---

\--- task \--- Aggiungi il tuo nuovo blocco personalizzato allo script Stage prima della fine dello script.

![Stage sprite](images/stage-sprite.png)

```blocks3
quando il flag ha fatto clic su
set [lives v] su (3)
set [punteggio v] su (0)
aspetta fino a <(lives) < (1)>

+ controlla high score :: custom
stop [all v]
```

\--- /compito \---

\--- compito \---

Fate il vostro gioco due volte per verificare se il tuo punteggio viene correttamente salvato come `punteggio`{: class = "block3variables"}.

\--- /compito \---