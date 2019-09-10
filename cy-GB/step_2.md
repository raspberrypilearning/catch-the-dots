## Creu rheolwr

Fe wnawn ni ddechrau trwy greu rheolwr, fydd yn cael ei ddefnyddio i gasglu’r dotiau.

--- task --- Agora'r prosiect cychwynnol Scratch 'Dal dotiau'.

**Arlein:** agora brosiect Scratch newydd yma [rpf.io/dots-on](http://rpf.io/dots-on){:target="_blank"}.

Os oes ganddot ti gyfrif Scratch galli di wneud copi drwy glicio ar **Remix**.

**All-lein:** lawrlwytha'r prosiect cychwynnol o [rpf.io/p/cy-GB/catch-the-dots-go](http://rpf.io/p/cy-GB/catch-the-dots-go) ac yna ei agor gan ddefnyddio'r golygydd all-lein.

Os oes angen i ti lawrlwytho a gosod golygydd Scratch all-lein, mae modd dod o hyd iddo yma [rpf.io/scratchoff](http://rpf.io/scratchoff).

--- /task ---

Fe ddyle ti weld ciplun rheolwr:

![sgrinlun](images/dots-controller.png)

--- task ---
Ychwanega gôd i dy reolwr fel fod y corlun yn troi i’r dde pan fyddi di’n gwasgu y bysell saeth dde:

![Corlun rheolwr](images/controller-sprite.png)

```blocks3
    pan fo'r flag werdd yn cael ei glicio
am byth 
  os <bysell (saeth de v) wedi ei phwyso?> yna 
    troi (3) gradd i'r dde
  end
end
```

--- /task ---

--- task --- Profa dy gôd. Fe ddylai dy reolwr droi i’r dde pan wyt ti'n gwasgu'r bysell saeth dde. --- /task ---

--- task --- Ychwanega gôd i dy reolwr fel fod y corlun yn troi i’r chwith pan fyddi di’n gwasgu y bysell saeth chwith.

![Corlun rheolwr](images/controller-sprite.png)

--- hints ---
 --- hint ---

Tyrd o hyd i'r côd sydd yn gwirio os yw'r botwm saeth dde wedi ei wasgu a gwneud i'r corlun droi i'r dde. Wyt ti'n gallu copio'r côd yma, a newid y copi fel ei fod yn gwirio os yw'r saeth chwith wedi ei wasgu i wneud i'r corlun droi i'r chwith?

--- /hint --- --- hint --- Dyma'r blociau rwyt ti eu hangen:

```blocks3
<bysell (bwlch v) wedi ei phwyso?>

troi (15) gradd i'r chwith

os <> yna
end
```

--- /hint --- --- hint --- Dyma sut ddylai dy gôd edrych:

```blocks3
    pan fo'r flag werdd yn cael ei glicio
    am byth 
        os <bysell (saeth de v) wedi ei phwyso?> yna 
          troi (3) gradd i'r dde
        end
+       os <bysell (saeth chwith v) wedi ei phwyso?> yna 
          troi (3) gradd i'r chwith
        end
    end
```

--- /hint --- --- /hints --- --- /task ---