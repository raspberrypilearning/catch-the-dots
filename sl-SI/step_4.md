## Več pik

--- task ---

Dvakrat podvoji figuro pike 'rdeča' in novi figuri poimenuj 'rumena' in 'modra'.

![posnetek zaslona](images/dots-more-dots.png)

--- /task ---

--- task ---

Spremeni videz novih figur, da bosta prave barve: 'rumena' naj bo rumena, 'modra' naj bo modra.

--- /task ---

--- task ---

Spremeni kodo obeh figur na način. da bo igralec moral ujeti dvojnika pike s pravilno barvo krmila, da bi dobil točke.

![posnetek zaslona](images/dots-all-test.png)

--- hints ---


--- hint ---

To je koda, ki jo moraš poiskati in prilagoditi figurama:

![posnetek zaslona](images/dots-more-dots.png)

```blocks3
      če <se dotika barve [#FF0000]?>
    spremeni [točke v] za (1)
    predvajaj zvok (pop) do konca
    ...
    konec
```

--- /hint ---

--- hint ---

Kodo za rumeno figuro moraš spremeniti na takšen način:

```blocks3
      če <se dotika barve [#FFFF00]? :: +> potem
    spremeni [točke v] za (1)
    predvajaj zvok (pop v)
  konec
```

Tako moraš spremeniti kodo za modro figuro:

```blocks3
    če <se dotika barve [#0000FF]? :: +> potem
    spremeni [točke v] za (1)
    predvajaj zvok (pop v)
  konec
```

--- /hint ---

--- /hints ---

--- /task ---

Če sedaj igraš svojo igro, boš videl, da da se pike včasih ustvarijo ena vrh druge.

--- task ---

Spremeni kodo za figuro pike 'rumena', da bo počakala štiri sekunde, po kliku na zastavico, preden se bo pojavila.

![Rumena pika](images/yellow-sprite.png)

```blocks3
    ko kliknemo na zastavico
  skrij
+   počakaj (4) sekund
```

![Modra pika](images/blue-sprite.png)

Nato spremeni kodo za figuro 'modra' pika, da bo počakala 6 sekund po kliku na zastavico, da se bo pojavila.

--- /task ---