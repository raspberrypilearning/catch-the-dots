## Ustvari krmilnik

Začni z ustvarjanjem krmila, ki ga bo igralev uporabljal za zbiranje pik.

--- task ---

Odpri začetni Scratch projekt 'Ujemi pike'.

**S povezavo:** odpri nov spletni Scratch projekt na [scratch.mit.edu/projects/397762613](https://scratch.mit.edu/projects/397762613){:target="_blank"}.

Če imaš Scratch uporabniški račun, lahko ustvariš kopijo s klikom na **Predelaj**.

**Brez povezave:** prenesi začetni projekt iz [rpf.io/p/sl-SI/catch-the-dots-go](https://rpf.io/p/sl-SI/catch-the-dots-go){:target="_blank"} in ga nato odpri s pomočjo namiznega urejevalnika.

Če želiš prenesti in namestiti Namizni Scratch, ga lahko najdeš na [rpf.io/scratchoff](https://rpf.io/scratchoff).

--- /task ---

Moral bi videti figuro krmila. Preimenuj jo v 'krmilo'.

![posnetek zaslona](images/dots-controller.png)

--- task ---

Figuri krmila dodaj kodo, ki povzroči, da se krmilo obrača v desno, ko igralec pritisne desno smerno tipko:

![Figura krmila](images/controller-sprite.png)

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

Preveri svojo kodo. Krmilo bi se morao obračati v desno, kadar pritisneš desno smerno tipko.

--- /task ---

--- task ---

Figuri krmila dodaj kodo, ki povzroči, da se krmilo obrača v levo, ko igralec pritisne levo smerno tipko.

![Figura krmila](images/controller-sprite.png)

--- hints ---


--- hint ---

Najdi kodo, ki preverja ali je pritisnjena desna smerna tipka in ki povzroči, da se figura obrača v desno. Ali lahko dodaš kopijo te kode in jo spremeniš na način, da bo preizkusila ali je pritisnjena leva smerna tipka in bo obračala obračanje figure v levo?

--- /hint ---

--- hint ---

To so potrebni bloki:

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

--- /hint ---

--- hint ---

Tvoja koda naj bi izgledala tako:

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
