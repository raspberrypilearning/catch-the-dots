## Pridobi točke ali izgubi življenje

Sedaj boš dodal nekaj pik, ki mora igralec zbirati.

--- task ---

Ustvari novo figuro, imenovano 'rdeča'. Ta figura bi morala biti mala rdeča pika.

![Figura rdeče pike](images/dots-red.png)

--- /task ---

--- task ---

Figuri 'rdeča' dodaj sledeče ukaze, da bi vsakih nekaj sekund ustvaril dvojnika figure:

![Figura rdeče pike](images/red-sprite.png)

```blocks3
    ko kliknemo na zastavico
  skrij
  počakaj (2) sekund
  ponavljaj
    usvari dvojnika (sebe v)
    počakaj (naključno število med (1) in (10)) sekund
  konec
```

--- /task ---

Če sedaj klikneš na zeleno zastavico, se zdi, kot da se ni zgodilo ničesar. Razlog je v temu, da so vsi dvojniki figure skriti in da se vsi nahajajo na istem mestu.

Sedaj boš dodal kodo, ki bo poskrbela, da se bo vsak nov dvojnik pojavil v enem od štirih kotov odra.

![posnetek zaslona](images/dots-start.png)

--- task ---

Ustvari nov seznam in ga poimenuj `začetne pozicije`{:class="block3variables"}. Klikni na `(+)` ikono seznama, da dodaš vrednosti `-180`{:class="block3variables"} in `180`{:class="block3variables"}.

![Figura rdeče pike](images/red-sprite.png)

![Seznam števil 180 in -180](images/dots-list.png)

[[[generic-scratch3-make-list]]]

Nato lahko skriješ seznam, tako da odznačiš ta kvadratek:

![Skrij seznam](images/hide-list.png)

--- /task ---

Opazil boš, da sta koordinati za vsak kot odra kombinaciji števil `180` in `-180`. To pomeni, da lahko uporabiš seznam, za naključno izbiranje kota odra.

--- task ---

Dodaj to kodo v figuro 'pika', da se vsak dovjnik figure pojavi v naključno izbranem kotu in se nato počasi ponika proti figuri krmila.

![Figura rdeče pike](images/red-sprite.png)

```blocks3
    ko začnem kot dvojnik
  pojdi na x: (element (naključno število med (1) in (2) v [začetne pozicije v]) y: (element (naključno število med (1) in (2)) v [začetne pozicije v])
  obrni se proti (krmilo v)
  pokaži
  ponavljaj do <se dotika (krmilo)?>
    pojdi (1) korakov
  konec
```

--- /task ---

Ta nova koda izbere ali `-180` ali `180` za naslednji x in y poziciji, kar pomeni, da vsak dvojnik 'pike' začne svojo pot v enem od kotov odra.

--- task ---

Preizkusi projekt. Moral bi videti rdeče pike, ki se pojavljajo v kotih odra in se počasi pomikajo proti krmilu.

![posnetek zaslona](images/dots-red-test.png)

--- /task ---

--- task ---

Ustvari dve novi spremenljivki imenovani `življenja`{:class="block3variables"} in `točke`{:class="block3variables"}.

![Figura rdeče pike](images/red-sprite.png)

--- /task ---

--- task ---

Odru dodaj kodo, ki ob pričetku igre nastavi spremenljivko `življenja`{:class="block3variables"} na `3` in `točke`{:class="block3variables"} na `0`. 

![Figura odra](images/stage-sprite.png)

```blocks3
ko kliknemo na zastavico
nastavi [življenja v] na (3)
nastavi [točke v] na (0)
```

--- /task ---

--- task ---

Na konec programa odra dodaj še to kodo, ki bo končala igro, kadar igralec izgubi še zadnje življenje:

![Figura odra](images/stage-sprite.png)

```blocks3
    počakaj dokler ni <(življenja :: variables) < [1]>
    ustavi [vse v]
```

--- /task ---

Igralec bi moral dobivati točke, kadra ulovi pike in izgubljati življenja, kadar ne uspe uloviti pik. Piko lahko ujame le z tisim delom krmila, ki je barvno usklajen s piko.

--- task ---

Vrni se na ukaze v figuri 'rdeča' in dodaj nekaj blokov kode za ukazi, ki sledijo bloku `ko začnem kot dvojnik`{:class="block3control"}.

Najprej poskrbi, da se dvojnik pike `premakne 5 korakov`{:class="block3motion"}, zato da prekrije krmilo.

Potem dodaj kodo, ki bodisi doda `1` spremenljivki `točke`{:class="block3variables"}, če se barva pike ujema z barvo krmila, ko se dotakneta, bodisi odvzame `1` spremenljivki `življenja`{:class="block3variables"}, kadar se barvi ne ujemata.

[[[generic-scratch3-sound-from-library]]]

![Figura rdeče pike](images/red-sprite.png)

```blocks3
    pojdi (5) korakov
  če <se dotika barve [#FF0000]?> potem
    spremeni [točke v] za (1)
    predvajaj zvok (pop) do konca
  sicer
    spremeni [življenja v] za (-1)
    predvajaj zvok (Laser1 v) do konca
  konec
  zbriši tega dvojnika
```

--- /task ---

--- task ---

Preizkusi svojo igor in se prepričaj, da:

1. izgubiš življenje, če se barvi pike in krmila ne ujemata;
2. dobiš piko, če se barvi ujemata.

--- /task ---