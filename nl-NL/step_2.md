## Een controller maken

Begin met het maken van een controller die de speler gebruikt om stippen te verzamelen.

--- task ---

Open het 'Vang de stippen' Scratch startproject.

**Online**: open het online starter project op [rpf.io/dots-on](https://rpf.io/dots-on){:target="_blank"}.

Als je een Scratch-account hebt, kun je een kopie maken door op **Remix** te klikken.

**Offline:** download het starter project op [rpf.io/p/nl-NL/catch-the-dots-go](https://rpf.io/p/nl-NL/catch-the-dots-go){:target="_blank"} en open het vervolgens met behulp van de Scratch offline editor.

Als je de Scratch offline editor wilt downloaden en installeren dan kan je die vinden op [rpf.io/scratchoff](https://rpf.io/scratchoff).

--- /task ---

Je zou een controller sprite moeten zien:

![schermafbeelding](images/dots-controller.png)

--- task ---

Voeg wat code toe aan de controller sprite om de sprite naar rechts te laten draaien als de speler op de rechter pijltjestoets klikt:

![Controller sprite](images/controller-sprite.png)

```blocks3
    when flag clicked
	  forever
		  if <key (right arrow v) pressed?> then
			  turn right (3) degrees
		  end
	  end
```

--- /task ---

--- task ---

Test je code. De controller sprite zou naar rechts moeten draaien wanneer je op de rechter pijltjestoets drukt.

--- /task ---

--- task ---

Voeg code toe aan de controller sprite om de sprite naar links te laten draaien als de speler op de linker pijltjestoets klikt.

![Controller sprite](images/controller-sprite.png)

--- hints ---


--- hint ---

Zoek de code die controleert of de rechter pijltjestoets is ingedrukt en de sprite naar rechts doet draaien. Kun je een kopie van deze code toevoegen en de kopie aanpassen zodat deze controleert of de linker pijltjestoets is ingedrukt en de sprite naar links doet draaien?

--- /hint ---

--- hint ---

Dit zijn de blokken die je nodig hebt:

```blocks3
<key (space v) pressed?>

draai (15) graden naar links

als <> dan

end
```

--- /hint ---

--- hint ---

Zo zou je code eruit moeten zien:

```blocks3
    when flag clicked
	  forever
		  if <key (right arrow v) pressed?> then
			  turn right (3) degrees
		  end
+ 		if <key (left arrow v) pressed?> then
			  turn left(3) degrees
		  end
	  end
```

--- /hint ---

--- /hints ---

--- /task ---
