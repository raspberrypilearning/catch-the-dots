## Meer stippen

--- task ---

Dupliceer tweemaal je 'rode' stip sprite en noem de twee nieuwe sprites 'geel' en 'blauw'.

![schermafbeelding](images/dots-more-dots.png)

--- /task ---

--- task ---

Verander het uiterlijk van elke nieuwe sprite zodat het de juiste kleur heeft: de 'gele' sprite moet geel zijn, de 'blauwe' sprite moet blauw zijn.

--- /task ---

--- task ---

Verander de code van elke sprite zodat de speler de stip kloon op de juiste kleur op de controller moet plaatsen om punten te scoren.

![schermafbeelding](images/dots-all-test.png)

--- hints ---


--- hint ---

Dit is de code die je nodig hebt voor het vinden en veranderen voor beide nieuwe sprites:

![schermafbeelding](images/dots-more-dots.png)

```blocks3
    if <touching color [#FF0000]?> then
		  change [score v] by (1)
		  play sound (pop v)
    end
```

--- /hint ---

--- hint ---

Zo verander je de code voor de gele sprite:

```blocks3
	if <touching color [#FFFF00]? :: +> then
        change [score v] by (1)
        play sound (pop v)
	end
```

Dit is hoe je de code voor de blauwe sprite moet veranderen:

```blocks3
	if <touching color [#0000FF]? :: +> then
        change [score v] by (1)
        play sound (pop v)
	end
```

--- /hint ---

--- /hints ---

--- /task ---

Als je het spel nu speelt, kun je zien dat de puntjes soms boven op elkaar worden geplaatst.

--- task ---

Verander de code voor de 'gele' stip sprite zodat het vier seconden wacht met verschijnen als op de groene vlag is geklikt.

![Gele stip](images/yellow-sprite.png)

```blocks3
	when flag clicked
	hide
+	wait (4) seconds
```

![Blauwe stip](images/blue-sprite.png)

Wijzig vervolgens de code voor de 'blauwe' stip sprite zodat deze 6 seconden wacht nadat op de groene vlag is geklikt voordat de sprite verschijnt.

--- /task ---
