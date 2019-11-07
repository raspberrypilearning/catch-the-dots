## Budowa pokrętła

Zacznij od stworzenia pokrętła-kontrolera, którego gracz będzie używał do zbierania kropek.

\---task\--- Otwórz projekt początkowy 'Łapanie kropek'.

**Online:** otwórz nowy projekt Scratcha na stronie [rpf.io/dots-on](http://rpf.io/dots-on){:target="_blank"}.

Jeśli posiadasz konto Scratch, możesz wykonać kopię klikając **Remix**.

**Offline:** pobierz projekt początkowy z [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go), i otwórz w programie Scratch Desktop.

Jeśli musisz pobrać i zainstalować edytor Scratcha, znajdziesz go na stronie [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /task \---

Powinieneś widzieć duszka kontrolera:

![zrzut ekranu](images/dots-controller.png)

\---task\--- Dodaj fragment kodu do duszka pokrętła aby duszek obracał się w prawo, jeśli gracz naciśnie strzałkę w prawo:

![Duszek pokrętła](images/controller-sprite.png)

```blocks3
    kiedy kliknięto flagę
      zawsze
        jeżeli <key (right arrow v) pressed?> to
          obróć w prawo o (3) stopni
        koniec
      koniec
```

\--- /task \---

\---task\--- Wypróbuj swój kod. Pokrętło powinno się obracać w prawo, kiedy naciśniesz strzałkę w prawo. \--- /task \---

\--- task \--- Dodaj kod do duszka pokrętła aby obracał się w lewo jeżeli gracz naciśnie strzałkę w lewo.

![Duszek pokrętła](images/controller-sprite.png)

\--- hints \--- \--- hint \---

Poniżej znajdziesz kod, który sprawdza czy strzałka w prawo jest wciśnięta i wtedy obraca duszka w prawo. Czy możesz dodać kopię tego kodu i zmienić go tak, aby sprawdzał kiedy wciśnięto strzałkę w lewo i obracał wtedy duszka w lewo?

\--- /hint \--- \--- hint \--- Poniżej masz bloczki, które będziesz potrzebować:

```blocks3
<key (space v) pressed?>

obróć w lewo o (15) stopni

jeżeli <> to

koniec
```

\--- /hint \--- \--- hint \--- Tak powinien wyglądać twój kod:

```blocks3
    kiedy kliknięto zieloną flagę
zawsze 
  jeżeli <key (right arrow v) pressed?> to 
    obróć w prawo o (3) stopni
  koniec
  + jeżeli <key (left arrow v) pressed?> to 
      obróć w lewo o (3) stopni
      koniec
koniec
```

\--- /hint \--- \--- /hints \--- \--- /task \---