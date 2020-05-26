## Υψηλό Σκορ

Πρόκειται να αποθηκεύεις το υψηλότερο σκορ έτσι ώστε οι παίκτες να μπορούν να δουν πόσο καλά τα καταφέρνουν.

\--- task \---

Δημιούργησε μία νέα μεταβλητή με όνομα `σκορ`{:class="block3variables"}.

![Stage sprite](images/stage-sprite.png)

\--- /task \---

\--- task \---

Επίλεξε το Σκηνικό. Κάνε κλικ στο 'Οι εντολές μου' και δημιούργησε ένα νέο μπλοκ με όνομα `έλεγξε υψηλό σκορ`{:class="block3myblocks"}.

![Stage sprite](images/stage-sprite.png)

![screenshot](images/dots-custom-1.png)

\--- /task \---

\--- task \---

Πρόσθεσε κώδικα στο δικό σου μπλοκ ώστε να ελέγχει αν η τρέχουσα τιμή της μεταβλητής `σκορ`{:class="block3variables"} είναι μεγαλύτερη από την τιμή της μεταβλητής `υψηλό σκορ`{:class="block3variables"} και στη συνέχεια να αποθηκεύει την τιμή του `σκορ`{:class="block3variables"} ως τη νέα τιμή του `υψηλό σκορ`{:class="block3variables"}.

![Stage sprite](images/stage-sprite.png)

```blocks3
    define check high score
    if <(score :: variables) > (high score)> then
        set [high score v] to (score :: variables)
    end
```

\--- /task \---

\--- task \---

Πρόσθεσε το νέο σου μπλοκ στον κώδικα του Σκηνικού πριν το τέλος του.

![Stage sprite](images/stage-sprite.png)

```blocks3
when flag clicked
set [lives v] to (3)
set [score v] to (0)
wait until <(lives) < (1)>

+ check high score :: custom
stop [all v]
```

\--- /task \---

\--- task \---

Play your game twice to check whether your score gets correctly saved as the `high score`{:class="block3variables"}.

\--- /task \---