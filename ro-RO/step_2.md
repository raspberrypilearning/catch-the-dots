## Creați un controler

Începeți prin crearea unui controler pe care playerul îl va folosi pentru a colecta puncte.

\--- task \--- Deschideți proiectul de "Scratch starter" "Catch the dots".

**Online:** open the starter project at [rpf.io/dots-on](http://rpf.io/dots-on){:target="_blank"}.

Dacă ai un cont Scratch, poți să creezi o copie dând click pe **Remix**.

**Offline:** download the starter project from [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go), and then open it in the Scratch offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /proba\---

Ar trebui să vedeți un controler pentru personaj:

![captură de ecran](images/dots-controller.png)

\--- task \--- Add some code to the controller sprite to make the sprite turn right if the player presses the right arrow key:

![Controller sprite](images/controller-sprite.png)

```blocks3
    when flag clicked
    forever
        if <key (right arrow v) pressed?> then
            turn right (3) degrees
        end
    end
```

\--- /task \---

\--- task \--- Test your code. The controller should spin to the right when you press the right arrow key. \--- /task \---

\--- task \--- Add code to the controller sprite to make the sprite turn left if the player presses the left arrow key.

![Controller sprite](images/controller-sprite.png)

\--- hints \--- \--- hint \---

Find the code that checks whether the right arrow key is pressed and makes the sprite turn right. Can you add a copy of this code, and change the copy so it checks whether the left arrow key is pressed and makes the sprite turn left?

\--- /hint \--- \--- hint \--- Here are the blocks you need:

```blocks3
<key (space v) pressed?>

viraj la stânga (15) grade

dacă <> apoi

sfârșit
```

\--- /hint \--- \--- hint \--- Here is what your code should look like:

```blocks3
    când steagul a dat clic
    pentru totdeauna
        dacă <key (right arrow v) pressed?> apoi
            virați dreapta (3) grade
        sfârșitul

+ dacă <key (left arrow v) pressed?> apoi
            virați la stânga (3) grade
        sfârșitul
    sfârșitul
```

\--- /hint \--- \--- /hints \--- \--- /task \---