## Creați un controler

Începeți prin crearea unui controler pe care playerul îl va folosi pentru a colecta puncte.

\--- task \--- Deschideți proiectul de "Scratch starter" "Catch the dots".

**Online:** deschideți proiectul starter la [rpf.io/dots-on](http://rpf.io/dots-on){: target = "_ blank"}. Dacă aveți un cont Scratch, puteți face clic pe **Remix** în colțul din dreapta sus pentru a salva o copie a proiectului.

**Offline:** descărcați proiectul starter din [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go), apoi deschideți-l în editorul Scratch offline.

Dacă trebuie să descărcați și să instalați editorul Scratch offline, îl puteți găsi la [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /task \---

Ar trebui să vedeți un controler pentru personaj:

![captură de ecran](images/dots-controller.png)

\--- task \--- Adăugați un anumit cod la sprite-ul controlerului pentru a transforma Sprite-ul în dreapta dacă jucătorul apasă tasta săgeată dreapta:

![Controler sprite](images/controller-sprite.png)

```blocks3
    when flag clicked
    forever
        if <key (right arrow v) pressed?> then
            turn right (3) degrees
        end
    end
```

\--- /task \---

\--- task \--- Testați-vă codul. Controlerul trebuie să se rotească spre dreapta atunci când apăsați tasta săgeată dreapta. \--- /task \---

\--- task \--- Adăugați codul la sprite-ul controlerului pentru a face sprite să se deplaseze stânga dacă jucătorul apasă tasta săgeată stânga.

![Controler sprite](images/controller-sprite.png)

\--- Sugestii \--- \--- Indicație \---

Găsiți codul care verifică dacă tasta săgeată dreapta este apăsată și face spriorul să meargă la dreapta. Puteți să adăugați o copie a acestui cod și să schimbați copia, astfel încât să verifice dacă tasta săgeată stânga este apăsată și face sprite să meargă la stânga?

\--- / hint \--- \--- indiciu \--- Aici sunt blocurile de care ai nevoie:

```blocks3
<key (space v) pressed?>

viraj la stânga (15) grade

dacă <> apoi

sfârșit
```

\--- / hint \--- \--- sugestie \--- Aici este ceea ce ar trebui să arate codul dvs.:

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

\--- / indiciu \--- \--- / sugestii \--- \--- / sarcina \---