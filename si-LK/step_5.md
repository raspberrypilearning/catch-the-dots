## අපහසු බව වෑඩි කර ගන්න

දැන් ඔබ ක්‍රීඩාව වඩාත් අපහසු කිරීමට යන්නේ ක්‍රීඩකයා එය ක්‍රීඩා කරන කාලය වෑඩි කරන විටය කාලයත් සමඟ තිත් වේගයෙන් දිස්වීමෙන් ඔබ මෙය කරනු ඇත.

\--- task \---

Create a new `variable`{:class="block3variables"} called 'delay'.

![Stage sprite](images/stage-sprite.png)

\--- /task \---

\--- task \---

Go to the Stage's Scripts area and create a new script that sets the `delay`{:class="block3variables"} variable to `8` and then slowly reduces the value of `delay`{:class="block3variables"} while the game runs.

![Stage sprite](images/stage-sprite.png)

```blocks3
    when flag clicked
    set [delay v] to (8)
    repeat until < (delay) = (2)>
        wait (10) seconds
        change [delay v] by (-0.5)
    end
```

\--- /task \---

Notice that this code is very similar to the code you would use to create a countdown timer!

Next, use the `delay`{:class="block3variables"} variable in the code scripts of the 'red', 'yellow', and 'blue' sprites.

\--- task \---

Remove the code block that makes the game wait a random number of seconds between making the dot sprite clones. Replace the block you've removed with your new `delay`{:class="block3variables"} variable:

![screenshot](images/all-dots.png)

```blocks3
<br />-   wait (pick random (5) to (10)) secs
    wait (delay :: variables) secs
```

Do this for all three dot sprites.

\--- /task \---

\--- task \---

Test the game, and check whether the dots begin to appear more quickly as the game goes on.

+ Does this work for all three coloured dots?
+ Can you see that the value of the `delay`{:class="block3variables"} variable decreases?

\--- /task \---