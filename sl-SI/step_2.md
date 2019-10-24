## Ustvari krmilnik

Začni z ustvarjanjem krmila, ki ga bo igralev uporabljal za zbiranje pik.

\--- task \--- Odpri začetni Scratch projekt 'Ujemi pike'.

**S povezavo:** odpri nov spletni Scratch projekt na [rpf.io/dots-on](http://rpf.io/dots-on){:target="_blank"}.

Če imaš Scratch uporabniški račun, lahko ustvariš kopijo s klikom na **Predelaj**.

** Brez povezave: ** prenesi začetni projekt iz [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go) {: target = "_ blank"} in ga nato odpri s pomočjo namiznega urejevalnika.

Če želiš prenesti in namestiti Namizni Scratch, ga lahko najdeš na [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /task \---

Moral bi videti figuro krmila. Preimenuj jo v 'krmilo'.

![posnetek zaslona](images/dots-controller.png)

\--- task \--- Figuri krmila dodaj kodo, ki povzroči, da se krmilo obrača v desno, ko igralec pritisne desno smerno tipko:

![Figura krmila](images/controller-sprite.png)

```blocks3
    ko kliknemo na zastavico
  ponavljaj
    če <je pritisnjena tipka [puščica v desno v]?> potem
      obrni se za (3) stopinj desno
    konec
  konec
```

\--- /task \---

\--- task \--- Preizkusi svojo kodo. Krmilo bi se morao obračati v desno, kadar pritisneš desno smerno tipko. \--- /task \---

\--- task \--- Figuri krmila dodaj kodo, ki povzroči, da se krmilo obrača v levo, ko igralec pritisne levo smerno tipko.

![Controller sprite](images/controller-sprite.png)

\--- hints \--- \--- hint \---

Najdi kodo, ki preverja ali je pritisnjena desna smerna tipka in ki povzroči, da se figura obrača v desno. Ali lahko dodaš kopijo te kode in jo spremeniš na način, da bo preizkusila ali je pritisnjena leva smerna tipka in bo obračala obračanje figure v levo?

\--- /hint \--- \--- hint \--- To so bloki kode, ki jih potrebuješ:

```blocks3
<je pritisnjena tipka (puščica levo)?>

obrni se za (15) stopinj levo

če <> potem

end
```

\--- /hint \--- \--- hint \--- Tvoja koda bi morala izgledati tako:

```blocks3
    ko kliknemo na zastavico
  ponavljaj
    če <je pritisnjena tipka [puščica v desno v]?> potem
    obrni se za (3) stopinj v desno
  konec

+  če <je pritisnjena tipka [puščica v levov]?> potem
    obrni se za (3) stopinj v levo
  konec
konec
```

\--- /hint \--- \--- /hints \--- \--- /task \---