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
  if <touching color [#FF0000]?> then
		change [točke v] by (1)
		play sound (pop v)
    ...
	end
```

--- /hint ---

--- hint ---

Kodo za rumeno figuro moraš spremeniti na takšen način:

```blocks3
  if <touching color [#FFFF00]? :: +> then
    change [točke v] by (1)
    play sound (pop v)
	end
```

Tako moraš spremeniti kodo za modro figuro:

```blocks3
  if <touching color [#0000FF]? :: +> then
    change [točke v] by (1)
    play sound (pop v)
	end
```

--- /hint ---

--- /hints ---

--- /task ---

Če sedaj igraš svojo igro, boš videl, da da se pike včasih ustvarijo ena vrh druge.

--- task ---

Spremeni kodo za figuro pike 'rumena', da bo počakala štiri sekunde, po kliku na zastavico, preden se bo pojavila.

![Rumena pika](images/yellow-sprite.png)

```blocks3
    when flag clicked
	  hide
+	  wait (4) seconds
```

![Modra pika](images/blue-sprite.png)

Nato spremeni kodo za figuro 'modra' pika, da bo počakala 6 sekund po kliku na zastavico, da se bo pojavila.

--- /task ---