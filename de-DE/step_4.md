## Weitere Punkte

\--- Aufgabe \--- Dupliziere dein 'rotes' Sprite zweimal und benenne die beiden neuen Sprites 'gelb' und 'blau'.

![Bildschirmfoto](images/dots-more-dots.png) \--- / Aufgabe \---

\--- Aufgabe \--- Ändere das Kostüm jedes neuen Sprites so, dass es die richtige Farbe hat: Der gelbe Sprite sollte gelb sein und der blaue Sprite sollte blau sein. \--- / Aufgabe \---

\--- task \--- Ändere den Code jedes Sprites so, dass der Spieler die Punktfarbe auf dem Controller mit der richtigen Farbe vergleichen muss, um Punkte zu erzielen.

![Bildschirmfoto](images/dots-all-test.png)

\--- Hinweise \--- \--- Hinweis \--- Dies ist der Code, den Sie für beide neuen Sprites finden und ändern müssen:

![Bildschirmfoto](images/dots-more-dots.png)

```blocks3
    Wenn <touching color [#FF0000]?> dann
        [Score v] um (1)
        ändern, Sound abspielen (Pop v)
...
    Ende
```

\--- / Hinweis \--- \--- Hinweis \--- So müssen Sie den Code für das gelbe Sprite ändern:

```blocks3
    wenn <Farbe berührt [# FFFF00]? :: +> dann
        [Score v] um (1)
        ändern, um Sound (Pop v)
    abzuspielen
```

So müssen Sie den Code für das blaue Sprite ändern:

```blocks3
    wenn <Farbe berührt [# 0000FF]? :: +> dann
        [Score v] um (1)
        ändern, um Sound (Pop v)
    abzuspielen
```

\--- / Hinweis \--- \--- / Hinweise \--- \--- / Aufgabe \---

Wenn Sie das Spiel jetzt spielen, können Sie sehen, dass die Punkte manchmal übereinander erstellt werden.

\--- task \--- Ändern Sie den Code für das 'gelbe' Punkt-Sprite so, dass es vier Sekunden nach dem Klicken auf die Flagge wartet, bevor es erscheint.

![Gelber Punkt](images/yellow-sprite.png)

```blocks3
    Wenn die Flagge auf
    geklickt wurde, verstecke
und warte (4) Sekunden
```

![Blauer Punkt](images/blue-sprite.png)

Ändern Sie dann den Code für das "blaue" Punktsprite so, dass es 6 Sekunden nach dem Klicken auf die Flagge wartet, bevor es erscheint.

\--- / Aufgabe \---