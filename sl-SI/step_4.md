## Več pik

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
      če <se dotika barve [#FF0000]?>
    spremeni [točke v] za (1)
    predvajaj zvok (pop) do konca
    ...
    konec
```

\--- /hint \---

\--- hint \---

This is how you need to change the code for the yellow sprite:

```blocks3
      če <se dotika barve [#FFFF00]? :: +> potem
    spremeni [točke v] za (1)
    predvajaj zvok (pop v)
  konec
```

This is how you need to change the code for the blue sprite:

```blocks3
    če <se dotika barve [#0000FF]? :: +> potem
    spremeni [točke v] za (1)
    predvajaj zvok (pop v)
  konec
```

\--- /hint \---

\--- /hints \---

\--- /task \---

If you play the game now, you can see that the dots sometimes get created one top of each other.

\--- task \---

Change the code for the 'yellow' dot sprite so that it waits four seconds after the flag is clicked before appearing.

![Yellow dot](images/yellow-sprite.png)

```blocks3
    ko kliknemo na zastavico
  skrij
+   počakaj (4) sekund
```

![Blue dot](images/blue-sprite.png)

Then change the code for the 'blue' dot sprite so that it waits 6 seconds after the flag is clicked before appearing.

\--- /task \---