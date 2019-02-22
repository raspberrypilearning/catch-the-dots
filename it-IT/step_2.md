## Crea un controller

Inizia creando un controller che il giocatore utilizzerà per raccogliere punti.

\--- task \--- Apri il progetto di avvio Scratch 'Catch the punti'.

**Online:** apri il progetto di avvio su [rpf.io/dots-on](http://rpf.io/dots-on){: target = "_ blank"}. Se si dispone di un account Scratch, è possibile fare clic su **Remix** nell'angolo in alto a destra per salvare una copia del progetto.

**Offline:** scarica il progetto di avvio da [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go), quindi aprilo nell'editor offline di Scratch.

Se devi scaricare e installare l'editor offline di Scratch, puoi trovarlo su [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /compito \---

Dovresti vedere uno sprite del controller:

![immagine dello schermo](images/dots-controller.png)

\--- task \--- Aggiungi del codice allo sprite del controller per far girare lo sprite a destra se il giocatore preme il tasto freccia destra:

![Controller sprite](images/controller-sprite.png)

```blocks3
    quando la bandiera ha cliccato
    per sempre
        se <key (right arrow v) pressed?> poi
            giri a destra (3) gradi
        fine
    fine
```

\--- /compito \---

\--- task \--- Verifica il tuo codice. Il controller dovrebbe ruotare a destra quando si preme il tasto freccia destra. \--- /compito \---

\--- task \--- Aggiungi il codice allo sprite del controller per far girare lo sprite a sinistra se il giocatore preme il tasto freccia sinistra.

![Controller sprite](images/controller-sprite.png)

\--- suggerimenti \--- \--- suggerimento \---

Trova il codice che controlla se il tasto freccia destra è premuto e fa girare lo sprite a destra. Puoi aggiungere una copia di questo codice e cambiare la copia in modo che controlli se il tasto freccia sinistra è premuto e fa girare lo sprite a sinistra?

\--- / suggerimento \--- \--- suggerimento \--- Ecco i blocchi necessari:

```blocks3
<key (space v) pressed?>

gira a sinistra (15) gradi

se <> poi

fine
```

\--- / suggerimento \--- \--- suggerimento \--- Ecco come dovrebbe apparire il tuo codice:

```blocks3
    quando la bandiera ha cliccato
    per sempre
        se <key (right arrow v) pressed?> poi
            gira a destra (3) gradi
        fine

+ se <key (left arrow v) pressed?> poi
            gira a sinistra (3) gradi
        fine
    fine
```

\--- / suggerimento \--- \--- / suggerimenti \--- \--- / compito \---