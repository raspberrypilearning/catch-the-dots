## Guadagna punti o perdi vite

Ora aggiungerai alcuni puntini che il giocatore deve raccogliere.

\--- task \---

Crea un nuovo sprite chiamato 'rosso'. Questo sprite dovrebbe essere un piccolo punto rosso.

![Sprite puntino rosso](images/dots-red.png)

\--- /task \---

\--- task \---

Aggiungi questo script al tuo sprite 'rosso' per creare un nuovo clone dello sprite ogni tot secondi:

![Sprite puntino rosso](images/red-sprite.png)

```blocks3
    when flag clicked
    hide
    wait (2) seconds
    forever
        create clone of (myself v)
        wait (pick random (5) to (10)) secs
    end
```

\--- /task \---

Se fai clic sulla bandierina verde ora, sembra che non succeda nulla. Questo perché tutti gli sprite clonati sono nascosti, e appaiono nello stesso posto.

Si sta per aggiungere il codice per far apparire ogni nuovo clone in uno dei quattro angoli dello Stage.

![screenshot](images/dots-start.png)

\--- task \---

Crea una nuova lista chiamata `posizioni di inizio`{:class="block3variables"}, clicca sull'icona `(+)` della lista per aggiungere i valori `-180`{:class="block3variables"} e `180`{:class="block3variables"}.

![Sprite puntino rosso](images/red-sprite.png)

![Lista 180 e -180](images/dots-list.png)

[[[generic-scratch3-make-list]]]

Successivamente puoi nascondere la lista deselezionando questa casella:

![Nascondi la lista](images/hide-list.png)

\--- /task \---

Notare che la coordinata di ogni angolo dello Stage è una combinazione di `180` e `-180`. Ciò significa che è possibile utilizzare la lista per scegliere un angolo dello stadio a caso.

\--- task \---

Aggiungi questo codice allo sprite 'punto' per far apparire ogni nuovo clone di sprite in un angolo casuale e poi lentamente muoversi verso lo sprite del controller.

![Sprite puntino rosso](images/red-sprite.png)

```blocks3
    when I start as a clone
    go to x: (item (pick random (1) to (2)) of [start positions v]) y: (item (pick random (1) to (2)) of [start positions v])
    point towards (controller v)
    show
    repeat until <touching (controller v)?>
        move (1) steps
    end
```

\--- /task \---

Questo nuovo codice sceglie `-180` o `180` per le posizioni x e y, in modo che ogni clone dello sprite 'punto' parta da un angolo dello Stage.

\--- task \---

Prova il tuo progetto. Dovresti vedere i puntini rossi apparire negli angoli dello Stage e muoversi lentamente verso il controller.

![screenshot](images/dots-red-test.png)

\--- /task \---

\--- task \---

Crea due nuove variabili chiamate `vite`{:class="block3variables"} e `punteggio`{:class="block3variables"}.

![Sprite puntino rosso](images/red-sprite.png)

\--- /task \---

\--- task \---

Aggiungi il codice allo Stage per impostare la variabile delle `vite`{:class="block3variables"} a ` 3 ` e il `punteggio`{:class="block3variables"} a `0` all'inizio del gioco. ![Sprite dello Stage](images/stage-sprite.png)

```blocks3
when flag clicked
set [lives v] to (3)
set [score v] to (0)
```

\--- /task \---

\--- task \---

Aggiungi questo codice alla fine dello script dello Stage per far terminare la partita quando il giocatore perde l'ultima vita:

![Sprite dello Stage](images/stage-sprite.png)

```blocks3
    wait until <(lives :: variables) < [1]>
    stop [all v]
```

\--- /task \---

Il giocatore dovrebbe aumentare il punteggio quanto cattura i puntini e perde vite in caso contrario. Un punto può essere catturato solo se il colore del controller corrisponde al colore del puntino.

\--- task \---

Torna negli script dello sprite puntino 'rosso' per aggiungere alcuni blocchi di codice alla fine dei comandi collegati a `quando vengo clonato`{:class="block3control"}.

Innanzitutto, fai che il clone si `sposti 5 passi`{:class="block3motion"} in modo che si sovrapponga al controller.

Quindi inserisci il codice per aggiungere `1` a `punteggio`{:class="block3variables"} se il colore del clone del punto corrisponde al colore del controller quando viene toccato, o togliere `1` a `vite`{:class="block3variables"} se i colori non coincidono.

[[[generic-scratch3-sound-from-library]]]

![Sprite puntino rosso](images/red-sprite.png)

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

Metti alla prova il tuo gioco per assicurarti che:

1. Perdi una vita se non abbini un punto al colore giusto
2. Ottieni un punto se abbini correttamente un puntino

\--- /task \---