## Erstelle einen Controller

Erstelle zunächst einen Controller, den der Spieler zum Sammeln von Punkten verwenden soll.

\--- task \---

Open the 'Catch the dots' Scratch starter project.

**Online:** open the starter project at [rpf.io/dots-on](https://rpf.io/dots-on){:target="_blank"}.

If you have a Scratch account you can make a copy by clicking **Remix**.

**Offline:** download the starter project from [rpf.io/p/en/catch-the-dots-go](https://rpf.io/p/en/catch-the-dots-go), and then open it in the Scratch offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff).

\--- /task \---

You should see a controller sprite:

![screenshot](images/dots-controller.png)

\--- task \---

Add some code to the controller sprite to make the sprite turn right if the player presses the right arrow key:

![Controller sprite](images/controller-sprite.png)

```blocks3
    wenn grüne Fahne angeklickt
    wiederhole fortlaufend
        falls <Taste ( Pfeil nach rechts v) gedrückt?> dann
            drehe dich rechts um (3) Grad
        Ende
    Ende
```

\--- /task \---

\--- task \---

Test your code. The controller should spin to the right when you press the right arrow key.

\--- /task \---

\--- task \---

Add code to the controller sprite to make the sprite turn left if the player presses the left arrow key.

![Controller sprite](images/controller-sprite.png)

\--- hints \---

\--- hint \---

Find the code that checks whether the right arrow key is pressed and makes the sprite turn right. Can you add a copy of this code, and change the copy so it checks whether the left arrow key is pressed and makes the sprite turn left?

\--- /hint \---

\--- hint \---

Here are the blocks you need:

```blocks3
<Taste ( Leertaste v) gedrückt?>

drehe dich links um (15) grad

wenn <> dann

Ende
```

\--- /hint \---

\--- hint \---

Here is what your code should look like:

```blocks3
    wenn grüne Fahne angeklickt
    wiederhole fortlaufend
        falls <Taste ( Pfeil nach rechts v) gedrückt?> dann
            drehe dich rechts um (3) Grad
        Ende

        falls <Taste ( Pfeil nach links v) gedrückt?> dann
            drehe dich links um (3) grad
        Ende
    Ende
```

\--- /hint \---

\--- /hints \---

\--- /task \---