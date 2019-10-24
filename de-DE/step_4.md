## Noch mehr Punkte

--- task --- Dupliziere deine 'rote' Figur zweimal und benenne die beiden neuen Figuren 'gelb' und 'blau'.

![Screenshot](images/dots-more-dots.png) --- /task ---

--- task --- Ändere das Kostüm jeder neuen Figur so, dass es die richtige Farbe hat: Die "gelb"-Figur sollte gelb sein und die "blau"-Figur sollte blau sein. --- /task ---

--- task --- Ändere den Code jeder Figur so, dass der Spieler den Controller so drehen muss, dass er den Punkt mit der entsprechenden Farbe fangen kann, um Punkte zu erzielen.

![Screenshot](images/dots-all-test.png)

--- hints ---
 --- hint --- Dies ist der Code, den du für beide neuen Figuren finden und ändern musst:

![Screenshot](images/dots-more-dots.png)

```blocks3
    falls <wird Farbe [#FF0000] berührt?> , dann 
        ändere [Punkte v] um (1)
        spiele Klang (pop v)
        ...
    end
```

--- /hint --- --- hint --- So musst du den Code für das gelbe Sprite ändern:

```blocks3
    falls <wird Farbe [#FFFF00] berührt? :: +> , dann 
        ändere [Punkte v] um (1)
        spiele Klang (pop v)
```

So musst du den Code für die blaue Figur ändern:

```blocks3
    falls <wird Farbe [#0000FF] berührt? :: +> , dann 
        ändere [Punkte v] um (1)
        spiele Klang (pop v)
```

--- /hint --- --- /hints --- --- /task ---

Wenn du das Spiel jetzt spielst, kannst du sehen, dass die Punkt-Figuren manchmal übereinander erstellt werden.

--- task --- Ändere den Code für die 'gelbe' Punkt-Figur so, dass sie nach dem Klicken auf die Flagge vier Sekunden wartet, bevor sie erscheint.

![Punkt-Figur gelb](images/yellow-sprite.png)

```blocks3
    Wenn die grüne Flagge angeklickt
    verstecke dich
+  warte (4) Sekunden
```

![Punkt-Figur blau](images/blue-sprite.png)

Ändere dann den Code für die "blaue" Punkt-Figur so, dass sie nach dem Klicken auf die Flagge 6 Sekunden wartet, bevor sie erscheint.

--- /task ---