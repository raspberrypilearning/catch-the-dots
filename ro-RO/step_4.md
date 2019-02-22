## Mai multe puncte

\--- task \--- Duplicați sprite-ul dvs. de culoare roșie de două ori și numiți cei doi noi "spanioli" și "albastri".

![captură de ecran](images/dots-more-dots.png) \--- /task \---

\--- task \--- Schimbați costumul fiecărui sprite nou, astfel că este culoarea corectă: Sprite-ul "galben" trebuie să fie galben, iar sprite-ul albastru ar trebui să fie albastru. \--- /task \---

\--- task \--- Schimbați codul fiecărui sprite astfel încât jucătorul trebuie să se potrivească cu clona dotată cu culoarea corectă a controlerului pentru a câștiga puncte.

![captură de ecran](images/dots-all-test.png)

\--- sugestii \--- \--- indiciu \--- Acesta este codul de care aveți nevoie pentru a găsi și modifica pentru ambele noi sprite:

![captură de ecran](images/dots-more-dots.png)

```blocks3
    dacă <touching color [#FF0000]?> atunci
        schimbă [scorul v] de (1)
        joacă sunetul (pop v)
...
    Sfârșit
```

\--- / hint \--- \--- hint \--- Așa trebuie să schimbi codul pentru sprite galben:

```blocks3
    dacă <atinge culoarea [# FFFF00]? :: +> apoi
        schimbare [scor v] prin (1)
        sunet de redare (pop v)
    sfarsit
```

Acesta este modul în care trebuie să modificați codul pentru sprite albastru:

```blocks3
    dacă <atinge culoarea [# 0000FF]? :: +> apoi
        schimbare [scor v] prin (1)
        sunet de redare (pop v)
    sfarsit
```

\--- / indiciu \--- \--- / sugestii \--- \--- / sarcina \---

Dacă joci acum jocul, poți vedea că punctele sunt uneori create unul peste celălalt.

\--- task \--- Schimbați codul pentru sprite-ul "galben", astfel încât să aștepte patru secunde după ce drapelul este apăsat înainte de a apărea.

![Punct galben](images/yellow-sprite.png)

```blocks3
    atunci când pavilionul a făcut clic pe
    ascundeți
+ așteptați (4) secunde
```

![Punct albastru](images/blue-sprite.png)

Apoi schimbați codul pentru sprite-ul albastru "albastru", astfel încât să aștepte 6 secunde după ce se face clic pe pavilion înainte de a apărea.

\--- /task \---