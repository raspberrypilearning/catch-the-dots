## Erhöhen Sie die Schwierigkeit

Jetzt wird das Spiel schwieriger, je länger der Spieler es spielt. Sie tun dies, indem Sie die Punkte mit der Zeit schneller und schneller erscheinen lassen.

\--- task \--- Erstellen Sie eine neue `Variable`{: class = "block3variables"} mit dem Namen 'delay'.

![Stage Sprite](images/stage-sprite.png) \--- / Aufgabe \---

Aufgabe Wechseln Sie zum Bereich Skripts der Bühne, und erstellen Sie ein neues Skript, das die Variable `delay`{: class = "block3variables"} auf `8` und dann den Wert von `delay`{langsam reduziert. class = "block3variables"} während das Spiel läuft.

![Stage Sprite](images/stage-sprite.png)

```blocks3
    Wenn das Flag auf
    geklickt ist, setzen Sie [delay v] bis (8)
    bis < (delay) = (2)>
        warten Sie (10) Sekunden
        ändern Sie [delay v] um (-0,5)
    end
```

\--- / Aufgabe \---

Beachten Sie, dass dieser Code dem Code sehr ähnlich ist, den Sie zum Erstellen eines Countdown-Timers verwenden würden!

Als nächstes verwenden Sie die Variable `delay`{: class = "block3variables"} in den Codeskripten der Sprites 'red', 'yellow' und 'blue'.

\--- task \--- Entferne den Code-Block, durch den das Spiel zwischen den Dot-Sprite-Klonen eine zufällige Anzahl von Sekunden warten muss. Ersetzen Sie den Block, den Sie entfernt haben, durch Ihre neue Variable `delay`{: class = "block3variables"}:

![Bildschirmfoto](images/all-dots.png)

```blocks3
<br />- warte (wähle zufällig (5) bis (10)) sek
    warte (delay :: variables) sek
```

Tun Sie dies für alle drei Punktsprites.

\--- / Aufgabe \---

Aufgabe Teste das Spiel und überprüfe, ob die Punkte im Laufe des Spiels schneller erscheinen.

+ Funktioniert das für alle drei farbigen Punkte?
+ Kannst du sehen, dass der Wert der `delay`{: class = "block3variables"} Variable abnimmt? \--- / Aufgabe \---