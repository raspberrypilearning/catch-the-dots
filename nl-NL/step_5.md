## Verhoog de moeilijkheid

Nu ga je het spel moeilijker maken naarmate de speler het langer speelt. Je doet dit door de stippen steeds sneller en sneller te laten verschijnen.

\--- task \---

Create a new `variable`{:class="block3variables"} called 'delay'.

![Stage sprite](images/stage-sprite.png)

\--- /task \---

\--- task \---

Go to the Stage's Scripts area and create a new script that sets the `delay`{:class="block3variables"} variable to `8` and then slowly reduces the value of `delay`{:class="block3variables"} while the game runs.

![Stage sprite](images/stage-sprite.png)

```blocks3
    wanneer groene vlag wordt aangeklikt
maak [vertraging v] (8)
herhaal tot < (vertraging) = (2)>
wacht (10) sec.
verander [vertraging v] met (-0.5)
end
```

\--- /task \---

Notice that this code is very similar to the code you would use to create a countdown timer!

Next, use the `delay`{:class="block3variables"} variable in the code scripts of the 'red', 'yellow', and 'blue' sprites.

\--- task \---

Remove the code block that makes the game wait a random number of seconds between making the dot sprite clones. Replace the block you've removed with your new `delay`{:class="block3variables"} variable:

![screenshot](images/all-dots.png)

```blocks3
<br />- wacht (willekeurig getal tussen (5) en (10)) sec.
wacht (vertraging) sec.
```

Do this for all three dot sprites.

\--- /task \---

\--- task \---

Test the game, and check whether the dots begin to appear more quickly as the game goes on.

+ Werkt dit voor alle drie gekleurde stippen?
+ Can you see that the value of the `delay`{:class="block3variables"} variable decreases?

\--- /task \---