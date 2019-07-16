## Tabela wyników

Zachowasz wysoki wynik gry, aby gracze mogli zobaczyć, jak dobrze sobie radzą.

\--- zadanie \--- Utwórz nową zmienną o nazwie `wysoki wynik`{: class = "block3variables"}.

![Duszek sceny](images/stage-sprite.png)

\--- /task \---

\--- zadanie \--- Wybierz scenę. Kliknij „Moje bloki” i utwórz nowy blok niestandardowy o nazwie `wysoki wynik`{: class = „block3myblocks”}.

![Duszek sceny](images/stage-sprite.png) ![zrzut ekranu](images/dots-custom-1.png)

\--- /task \---

\--- zadanie \--- Dodaj kod do swojego bloku niestandardowego, aby blok sprawdzał, czy bieżąca wartość ``{: class = "block3variables"} większą niż wartość `najwyższego wyniku`{: class = zmienna "block3variables"}, a następnie przechowuje wartość `wyników`{: class = "block3variables"} jako nowa wartość `high score`{: class = "block3variables"}.

![Duszek sceny](images/stage-sprite.png)

```blocks3
    zdefiniuj wynik wysoki wynik
    jeśli <(wynik :: zmienne) > (wynik wysoki)> a następnie
        ustaw [wynik wysoki v] na (wynik :: zmienne)
    koniec
```

\--- /task \---

\--- zadanie \--- Dodaj nowy blok niestandardowy do skryptu Stage przed końcem skryptu.

![Duszek sceny](images/stage-sprite.png)

```blocks3
po kliknięciu flagi
ustaw [życia v] na (3)
ustaw [wynik v] na (0)
czekaj do <(życia) < (1)>

+ sprawdź wysoki wynik :: niestandardowy
stop [wszystkie v]
```

\--- /task \---

\--- task \---

Zagraj w swoją grę dwa razy, aby sprawdzić, czy Twój wynik zostanie poprawnie zapisany jako `wysoki wynik`{: class = "block3variables"}.

\--- /task \---