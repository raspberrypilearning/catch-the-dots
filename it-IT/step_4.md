## Più punti

\--- task \---

Duplicate your 'red' dot sprite twice, and name the two new sprites 'yellow' and 'blue'.

![screenshot](images/dots-more-dots.png)

\--- /task \---

\--- task \---

Change the costume of each new sprite so it is the correct colour: the 'yellow' sprite should be yellow, and the 'blue' sprite should be blue.

\--- /task \---

\--- task \---

Change the code of each sprite so that the player has to match dot clone to the correct colour on the controller to score points.

![screenshot](images/dots-all-test.png)

\--- hints \---

\--- hint \---

This is the code you need to find and alter for both new sprites:

![screenshot](images/dots-more-dots.png)

```blocks3
    se <touching color [#FF0000]?> allora
        cambia [punteggio v] per (1)
        suono riprodotto (pop v)
...
    fine
```

\--- /hint \---

\--- hint \---

This is how you need to change the code for the yellow sprite:

```blocks3
    se <tocca il colore [# FFFF00]? :: +> quindi
        modifica [punteggio v] per (1)
        suono riproduzione (pop v)
    fine
```

This is how you need to change the code for the blue sprite:

```blocks3
    se <tocca il colore [# 0000FF]? :: +> quindi
        modifica [punteggio v] per (1)
        suono riproduzione (pop v)
    fine
```

\--- /hint \---

\--- /hints \---

\--- /task \---

If you play the game now, you can see that the dots sometimes get created one top of each other.

\--- task \---

Change the code for the 'yellow' dot sprite so that it waits four seconds after the flag is clicked before appearing.

![Yellow dot](images/yellow-sprite.png)

```blocks3
    quando il flag ha cliccato
    nascondi
+ aspetta (4) secondi
```

![Blue dot](images/blue-sprite.png)

Then change the code for the 'blue' dot sprite so that it waits 6 seconds after the flag is clicked before appearing.

\--- /task \---