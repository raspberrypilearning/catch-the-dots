## Creu rheolwr

Fe wnawn ni ddechrau trwy greu rheolwr, fydd yn cael ei ddefnyddio i gasglu’r dotiau.

\--- task \--- Agora'r prosiect cychwynnol Scratch 'Dal dotiau'.

**Arlein:** agora brosiect Scratch newydd yma [rpf.io/dots-on](http://rpf.io/dots-on){:target="_blank"}.

Os oes ganddot ti gyfrif Scratch galli di wneud copi drwy glicio ar ** Remix **.

** All-lein: ** lawrlwytha'r prosiect cychwynnol o [ rpf.io/p/en/catch-the-dots-go ](http://rpf.io/p/en/catch-the-dots-go) ac yna ei agor gan ddefnyddio'r golygydd all-lein.

Os oes angen i ti lawrlwytho a gosod golygydd Scratch all-lein, mae modd dod o hyd iddo yma [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /task \---

Fe ddyle ti weld ciplun rheolwr:

![sgrinlun](images/dots-controller.png)

Ychwanega gôd i dy reolwr fel fod y corlun yn troi i’r dde pan fyddi di’n gwasgu y bysell saeth dde:

![Corlun rheolwr](images/controller-sprite.png)

```blocks3
    when flag clicked
    forever
        if <key (right arrow v) pressed?> then
            turn right (3) degrees
        end
    end
```

\--- /task \---

\--- task \--- Profa dy gôd. Fe ddylai dy reolwr droi i’r dde pan wyt ti'n gwasgu'r bysell saeth dde. \--- /task \---

\--- task \--- Ychwanega gôd i dy reolwr fel fod y corlun yn troi i’r chwith pan fyddi di’n gwasgu y bysell saeth chwith.

![Corlun rheolwr](images/controller-sprite.png)

\--- hints \--- \--- hint \---

Tyrd o hyd i'r côd sydd yn gwirio os yw'r botwm saeth dde wedi ei wasgu a gwneud i'r corlun droi i'r dde. Wyt ti'n gallu copio'r côd yma, a newid y copi fel ei fod yn gwirio os yw'r saeth chwith wedi ei wasgu i wneud i'r corlun droi i'r chwith?

\--- /hint \--- \--- hint \--- Dyma'r blociau rwyt ti eu hangen:

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

\--- /hint \--- \--- hint \--- Dyma sut ddylai dy gôd edrych:

```blocks3
    when flag clicked
    forever
        if <key (right arrow v) pressed?> then
            turn right (3) degrees
        end

+       if <key (left arrow v) pressed?> then
            turn left(3) degrees
        end
    end
```

\--- /hint \--- \--- /hints \--- \--- /task \---