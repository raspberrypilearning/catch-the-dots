## Povečaj težavnost

Sedaj boš poskrbel, da bo igra postala težje, tem dlje jo igralec igra. To boš dosegel s tem, da se bodo pike pojavljale vedno hitreje.

\--- task \---

Create a new `variable`{:class="block3variables"} called 'delay'.

![Stage sprite](images/stage-sprite.png)

\--- /task \---

\--- task \---

Go to the Stage's Scripts area and create a new script that sets the `delay`{:class="block3variables"} variable to `8` and then slowly reduces the value of `delay`{:class="block3variables"} while the game runs.

![Stage sprite](images/stage-sprite.png)

```blocks3
    ko kliknemo na zastavico
  nastavi [zamik v] na (8)
  ponavljaj dokler  < (zamik) = (2)>
      počakaj (10) sekund
      spremeni [zamik v] za (-0.5)
  konec
```

\--- /task \---

Notice that this code is very similar to the code you would use to create a countdown timer!

Next, use the `delay`{:class="block3variables"} variable in the code scripts of the 'red', 'yellow', and 'blue' sprites.

\--- task \---

Remove the code block that makes the game wait a random number of seconds between making the dot sprite clones. Replace the block you've removed with your new `delay`{:class="block3variables"} variable:

![screenshot](images/all-dots.png)

```blocks3
<br />- počakaj (naključno število med (5) in (10)) sekund
  počakaj (zamik :: spremenljivke) sekund
```

Do this for all three dot sprites.

\--- /task \---

\--- task \---

Test the game, and check whether the dots begin to appear more quickly as the game goes on.

+ Ali to deluje za vse tri barve pik?
+ Can you see that the value of the `delay`{:class="block3variables"} variable decreases?

\--- /task \---