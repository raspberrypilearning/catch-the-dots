## Creare un controller

Iniziamo con il creare un controller che può essere usato per raccogliere i puntini.

\--- task \---

Apri il progetto di partenza Scratch 'Cattura i puntini'.

**Online:** open the starter project at [rpf.io/dots-on](https://rpf.io/dots-on){:target="_blank"}.

Se hai un account su Scratch, puoi farne una copia cliccando su **Remix**.

**Offline:** download the starter project from [rpf.io/p/en/catch-the-dots-go](https://rpf.io/p/en/catch-the-dots-go), and then open it in the Scratch offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff).

\--- /task \---

Dovresti vedere lo sprite di un controller:

![screenshot](images/dots-controller.png)

\--- task \---

Aggiungi del codice allo sprite del controller per farlo ruotare a destra se il giocatore preme il tasto freccia destra:

![Sprite del controller](images/controller-sprite.png)

```blocks3
    when flag clicked
    forever
        if <key (right arrow v) pressed?> then
            turn right (3) degrees
        end
    end
```

\--- /task \---

\--- task \---

Prova il tuo codice. Il controller dovrebbe ruotare a destra quando si preme il tasto freccia destra.

\--- /task \---

\--- task \---

Aggiungi il codice allo sprite del controller per farlo girare a sinistra se il giocatore preme il tasto freccia sinistra.

![Sprite del controller](images/controller-sprite.png)

\--- hints \---

\--- hint \---

Trova il codice che controlla se viene premuto il tasto freccia destra e che fa girare lo sprite a destra. Puoi aggiungere una copia di questo codice, e cambiarlo in modo da controllare se il tasto freccia sinistra è premuto e quindi faccia girare lo sprite a sinistra?

\--- /hint \---

\--- hint \---

Ecco i blocchi di codice che ti serviranno:

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

\--- /hint \---

\--- hint \---

Ecco come dovrebbe apparire il codice:

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

\--- /hint \---

\--- /hints \---

\--- /task \---