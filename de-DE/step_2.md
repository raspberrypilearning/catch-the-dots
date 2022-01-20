## Erstelle einen Controller

Erstelle zunächst einen Controller, den der Spieler zum Sammeln von Punkten verwenden soll.

--- task --- Öffne das Scratch-Basisprojekt 'Fang die Punkte'.

**Online:** öffne das Basisprojekt auf [rpf.io/dots-on](https://rpf.io/dots-on){:target="_blank"}.

Wenn du bereits einen Scratch-Account besitzt, kannst du dir durch klicken auf **Remix** eine Kopie anlegen.

**Offline:** Lade das Basisprojekt von [rpf.io/p/de-DE/catch-the-dots-go](https://rpf.io/p/de-DE/catch-the-dots-go) herunter und öffne es dann mit dem Scratch Offline-Editor.

Wenn du den Scratch-Offline-Editor herunterladen und installieren möchtest, findest du diesen unter [rpf.io/scratchoff](https://rpf.io/scratchoff).

--- /task ---

Du solltest einen Controller (Steuerungs-Figur) sehen:

![Bildschirmfoto](images/dots-controller.png)

--- task --- Füge Code zur Controller-Figur hinzu, damit sie sich rechts herum dreht, wenn die "Pfeil nach rechts" Taste gedrückt wird:

![Controller-Figur](images/controller-sprite.png)

```blocks3
    Wenn die grüne Flagge angeklickt
    wiederhole fortlaufend 
        falls <Taste (Pfeil nach rechts v) gedrückt?> , dann 
            drehe dich nach rechts um (3) Grad
```

--- /task ---

--- task --- Teste deinen Code. Der Controller sollte sich nach rechts drehen, wenn du die Taste "Pfeil nach rechts" drückst. --- /task ---

--- task --- Füge Code zur Controller-Figur hinzu, damit sie sich links herum dreht, wenn die "Pfeil nach links" Taste gedrückt wird.

![Controller-Figur](images/controller-sprite.png)

--- hints ---
 --- hint ---

Suche den Code, der prüft, ob die Taste "Pfeil nach rechts" gedrückt ist und der dafür sorgt, dass die Figur sich nach rechts dreht. Kannst du eine Kopie dieses Codes machen und ihn so abändern, dass er prüft, ob die Taste "Pfeil nach links" gedrückt wurde und der die Figur dann nach links drehen lässt?

--- /hint --- --- hint --- Hier sind die Code Blöcke die du brauchst:

```blocks3
<Taste (Leertaste v) gedrückt?>

drehe dich nach links um (15) Grad

falls <> , dann
```

--- /hint --- --- hint --- So sollte dein Code aussehen:

```blocks3
    Wenn die grüne Flagge angeklickt
    wiederhole fortlaufend 
        falls <Taste (Pfeil nach rechts v) gedrückt?> , dann 
            drehe dich nach rechts um (3) Grad
+       falls <Taste (Pfeil nach links v) gedrückt?> , dann 
            drehe dich nach links um (3) Grad
```

--- /hint --- --- /hints --- --- /task ---
