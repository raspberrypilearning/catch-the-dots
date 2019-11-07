## Zwiększenie trudności

Teraz zrobisz grę tym trudniejszą, im dłużej gracz w nią gra. Osiągniesz to sprawiając, że kropki pojawią się coraz szybciej z upływem czasu.

--- task --- Utwórz nową `zmienną`{:class="block3variables"} nazwaną 'opóźnienie'.

![Duszek sceny](images/stage-sprite.png) --- /task ---

--- task --- Przejdź do obszaru skryptu sceny i utwórz nowy skrypt, który ustawia zmienną `opóźnienie`{:class="block3variables"} na `8` a następnie powoli zmniejsza wartość zmiennej `opóźninie`{:class="block3variables"} podczas gry.

![Duszek sceny](images/stage-sprite.png)

```blocks3
    kiedy kliknięto zieloną flagę
    ustaw [opóźnienie v] na (8)
    powtarzaj aż <(opóźnienie) = (2)> 
        czekaj (10) sekund
        zmień [opóźnienie v] o (-0.5)
    koniec
```

--- /task ---

Zauważ, że ten kod jest bardzo podobny do kodu, którego użyłbyś do utworzenia minutnika!

Następnie użyj zmiennej `opóźnienie`{:class="block3variables"} w skryptach kodu „czerwonych”, „żółtych” i „niebieskich” ikonek.

--- task --- Usuń blok kodu, który sprawia, że gra czeka losową liczbę sekund między utworzeniem klonów kropek. Zastąp usunięty blok nową zmienną `opóźnienie`{:class="block3variables"}:

![zrzut ekranu](images/all-dots.png)

```blocks3
    czekaj (losuj liczbę od (5) do (10)) sekund
-   czekaj (opóźnienie :: variables) sekund
```

Zrób to dla wszystkich trzech duszków kropek.

--- /task ---

--- task --- Przetestuj grę i sprawdź, czy kropki zaczynają pojawiać się szybciej, gdy gra toczy się dłużej.

+ Czy to działa dla wszystkich trzech kolorów kropek?
+ Czy widzisz, że wartość zmiennej `opóźnienie`{:class="block3variables"} zmniejsza się? --- /task ---