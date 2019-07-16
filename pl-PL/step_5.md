## Zwiększenie trudności

Teraz utrudnisz grę, im dłużej gracz ją zagra. Zrobisz to, sprawiając, że kropki pojawią się szybciej i szybciej z upływem czasu.

\--- zadanie \--- Utwórz nową `zmienną`{: class = "block3variables"} zwaną 'delay'.

![Duszek sceny](images/stage-sprite.png) \--- /task \---

\--- task \--- Przejdź do obszaru Scripts Stage i utwórz nowy skrypt, który ustawia zmienną `delay`{: class = "block3variables"} na `8` a następnie powoli zmniejsza wartość `delay`{: class = "block3variables"} podczas gry.

![Duszek sceny](images/stage-sprite.png)

```blocks3
    po kliknięciu flagi
    ustaw [opóźnienie v] na (8)
    powtórz do < (opóźnienie) = (2)>
        poczekaj (10) sekund
        zmień [opóźnienie v] o (-0,5)
    koniec
```

\--- /task \---

Zauważ, że ten kod jest bardzo podobny do kodu, którego użyłbyś do utworzenia minutnika!

Następnie użyj zmiennej `delay`{: class = "block3variables"} w skryptach kodu „czerwonych”, „żółtych” i „niebieskich” ikonek.

\--- zadanie \--- Usuń blok kodu, który sprawia, że gra czeka losową liczbę sekund między utworzeniem klonów kropek. Zastąp usunięty blok nowym `opóźnieniem`{: class = "block3variables"} zmienną:

![zrzut ekranu](images/all-dots.png)

```blocks3
<br />- czekaj (wybierz losowe (5) do (10)) sek
    czekanie (opóźnienie :: zmienne) sek
```

Zrób to dla wszystkich trzech ikonek.

\--- /task \---

\--- zadanie \--- Przetestuj grę i sprawdź, czy kropki zaczynają pojawiać się szybciej, gdy gra toczy się dalej.

+ Czy to działa dla wszystkich trzech kolorowych kropek?
+ Czy widzisz, że wartość `opóźnienia`{: class = "block3variables"} zmniejsza się? \--- /task \---