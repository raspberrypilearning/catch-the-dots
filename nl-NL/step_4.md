## Meer stippen

\--- task \--- Dupliceer tweemaal je 'rode' stip sprite en noem de twee nieuwe sprites 'geel' en 'blauw'.

![screenshot](images/dots-more-dots.png) \--- /task \---

\--- task \--- Verander het uiterlijk van elke nieuwe sprite zodat het de juiste kleur heeft: de 'gele' sprite moet geel zijn en de 'blauwe' sprite moet blauw zijn. \--- /task \---

\--- task \--- Wijzig de code van elke sprite zodat de speler de stip clone moet paren met de juiste kleur op de controller om punten te scoren.

![screenshot](images/dots-all-test.png)

\--- hints \--- \--- hint \--- Dit is de code die je moet vinden en wijzigen voor beide nieuwe sprites:

![schermafdruk](images/dots-more-dots.png)

```blocks3
    als <raak ik kleur [FF0000]? > dan 
verander [score v] met (1)
start geluid (pop v)
...
    end :: control
```

\--- /hint \--- \--- hint \--- Dit is hoe je de code voor de gele sprite moet veranderen:

```blocks3
    als <raak ik kleur [#FFFF00]? :: +> dan
verander [score v] met (1)
start geluid (pop v)
end
```

Dit is hoe je de code voor de blauwe sprite moet veranderen:

```blocks3
    als <raak ik kleur [#0000FF]? :: +> dan
verander [score v] met (1)
start geluid (pop v)
end
```

\--- /hint \--- \--- /hints \--- \--- /task \---

Als je het spel nu speelt, kun je zien dat de puntjes soms boven op elkaar worden gemaakt.

\--- task \--- Wijzig de code voor de 'gele' stip-sprite zodat deze vier seconden wacht nadat op de groene vlag is geklikt voordat deze wordt weergegeven.

![Gele stip](images/yellow-sprite.png)

```blocks3
    wanneer groene vlag wordt aangeklikt
verdwijn
+ wacht (4) sec.
```

![Blauwe stip](images/blue-sprite.png)

Wijzig vervolgens de code voor de 'blauwe' stip-sprite zodat deze 6 seconden wacht nadat op de groene vlag is geklikt voordat de sprite verschijnt.

\--- /task \---