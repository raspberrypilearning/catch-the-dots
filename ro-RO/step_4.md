## Colecteaza puncte

Să adăugăm câteva puncte pe care jucătorul să le adune cu controlerul lui.

+ Creaza un personaj numit 'ŕosu'. Acest personaj trebuie sa fie un mic punct rosu.
    
    ![screenshot](images/dots-red.png)

+ Adăugați acest script la personajulul "roșu", pentru a crea o nouă clonă a punctului rosu la fiecare câteva secunde:
    
    ```blocks
        when flag clicked
        hide
        wait (2) secs
        forever
            create clone of [myself v]
            wait (pick random (5) to (10)) secs
        end
    ```

+ Când fiecare clona este creată, doriți să apară într-unul din cele patru colțuri ale scenei.
    
    ![screenshot](images/dots-start.png)
    
    Pentru a face acest lucru, mai întâi creați o nouă **list** numita <`start positions`{:class="blockdata"} și faceți clic pe `(+)` pentru a adauga valorile `-180` si `180`.
    
    ![screenshot](images/dots-list.png)

+ Puteți utiliza aceste două elemente de listă pentru a alege un colț aleatoriu al scenei. Adăugați aceste linii de cod la personajul "punct", astfel încât fiecare clonă nouă să se deplaseze într-un colț aleatoriu și apoi să se mute încet spre controler.
    
    ```blocks
        when I start as a clone
        go to x: (item (random v) of [start positions v]) y: (item (random v) of [start positions v])
        point towards [controller v]
        show
        repeat until <touching [controller v]?>
            move (1) steps
        end
     
    
    ```
    
    Codul de mai sus alege `-180` sau `180` pentru pozițiile x * și * y, ceea ce înseamnă că fiecare clonă începe într-un colț al scenei.

+ Salvați proiectul. Ar trebui să vedeți multe puncte roșii în fiecare colț al ecranului care se mișca încet spre controler.
    
    ![screenshot](images/dots-red-test.png)

+ Create 2 new variables called `lives`{:class="blockdata"} and `score`{:class="blockdata"}.

+ Add code to your stage to set the `lives`{:class="blockdata"} to 3 and the `score`{:class="blockdata"} to 0 at the start of the game.

+ You need to add code to the end of your red dot's `when I start as a clone`{:class="blockcontrol"} code, so that either 1 is added to the player's `score`{:class="blockdata"} if the colours match, or 1 is taken from the player's `lives`{:class="blockdata"} if the colours don't match.
    
    ```blocks
        move (5) steps
        if <touching color [#FF0000]?> then
            change [score v] by (1)
            play sound [pop v]
        else
            change [lives v] by (-1)
            play sound [laser1 v]
        end
        delete this clone
    ```

+ Add this code to the end of your stage's script, so that the game ends when the player loses all of their lives:
    
    ```blocks
        wait until <(lives) < [1]>
        stop [all v]
    ```

+ Test your game to make sure this code works as expected.