## Υψηλό Σκορ

Πρόκειται να αποθηκεύεις το υψηλότερο σκορ έτσι ώστε οι παίκτες να μπορούν να δουν πόσο καλά τα καταφέρνουν.

\--- task \--- Δημιούργησε μία νέα μεταβλητή με όνομα `υψηλό σκορ`{:class="block3variables"}.

![Stage sprite](images/stage-sprite.png)

\--- /task \---

\--- task \--- Επέλεξε το Σκηνικό. Κάνε κλικ στο 'Οι εντολές μου' και δημιούργησε ένα νέο μπλοκ με όνομα `έλεγξε υψηλό σκορ`{:class="block3myblocks"}.

![Stage sprite](images/stage-sprite.png) ![screenshot](images/dots-custom-1.png)

\--- /task \---

\--- task \--- Πρόσθεσε κώδικα στο δικό σου μπλοκ ώστε να ελέγχει αν η τρέχουσα τιμή της μεταβλητής `σκορ`{:class="block3variables"} είναι μεγαλύτερη από την τιμή της μεταβλητής `υψηλό σκορ`{:class="block3variables"} και στη συνέχεια να αποθηκεύει την τιμή του `σκορ`{:class="block3variables"} ως τη νέα τιμή του `υψηλό σκορ`{:class="block3variables"}.

![Stage sprite](images/stage-sprite.png)

```blocks3
    ορισμός check high score
εάν <(score :: variables) > (high score)> τότε 
  όρισε [high score v] σε (score :: variables)
end
```

\--- /task \---

\--- task \--- Πρόσθεσε το νέο σου μπλοκ στον κώδικα του Σκηνικού πριν το τέλος του.

![Stage sprite](images/stage-sprite.png)

```blocks3
Όταν στην πράσινη σημαία γίνει κλικ
όρισε [lives v] σε (3)
όρισε [score v] σε (0)
περίμενε ώσπου <(lives) < (1)> < (1)>

+ check high score :: custom
σταμάτησε [all v]
```

\--- /task \---

\--- task --

Παίξε το παιχνίδι σου δύο φορές για να ελέγξεις ότι το σκορ αποθηκεύεται σωστά ως `υψηλό σκορ`{:class="block3variables"}.

\--- /task \---