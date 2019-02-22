## Cel mai mare scor

Veți salva scorul mare al jocului, astfel încât jucătorii să poată vedea cât de bine se fac.

\--- task \--- Creați o nouă variabilă numită `scor mare`{: class = "block3variables"}.

![Scena sprite](images/stage-sprite.png)

\--- /task \---

\--- task \--- Selectați etapa. Faceți clic pe "Blocurile mele" și creați un nou bloc personalizat, numit `verificați un scor mare`{: class = "block3myblocks"}.

![Scena sprite](images/stage-sprite.png) ![captură de ecran](images/dots-custom-1.png)

\--- /proba\---

\--- sarcina \--- Adauga codul la blocul personalizat , astfel încât controalele bloc dacă valoarea curentă a `scor`{: class = „block3variables“} în mai mare decât valoarea `scor`{: class = variabila "block3variables"} și apoi stochează valoarea de `scoruri`{: class = "block3variables"} ca noua valoare de `scoruri mari`{: class = "block3variables"}.

![Scena sprite](images/stage-sprite.png)

```blocks3
    definesc scorul mare de verificare
    dacă <(scor :: variabile) > (scor mare)> apoi
        set [scor mare v] la (scor :: variabile)
    sfârșit
```

\--- /task \---

\--- task \--- Adăugați noul bloc personalizat la scenariul Stage înainte de sfârșitul scriptului.

![Scena sprite](images/stage-sprite.png)

```blocks3
când pavilion apasat
set [trăiește v] până la (3)
set [scor v] până la (0)
așteptați până <(vieți) < (1)>

+ verifica scor :: personalizat
oprire [totul v]
```

\--- /task \---

\--- task \---

Joaca jocul de două ori pentru a verifica dacă scorul dvs. devine salvat corect ca `mare scor`{: class = „block3variables“}.

\--- /task \---