## Najboljši rezultat

Shranil boš najboljši rezultat, tako da bodo igralci vedeli, kako jim gre.

--- task ---

Ustvari novo spremenljivko imenovano `najboljši rezultat`{:class="block3variables"}.

![Figura odra](images/stage-sprite.png)

--- /task ---

--- task ---

Izberi oder. Klikni na 'Moji bloki' in ustvari nov blok imenovan `preveri najboljši rezultat`{:class="block3myblocks"}.

![Figura odra](images/stage-sprite.png)

![posnetek zaslona](images/dots-custom-1.png)

--- /task ---

--- task ---

Tvojemu bloku dodaj kodo, ki preveri ali je trenutna vrednost spremenljivke `točke`{:class="block3variables"} večja od vrednosti `najboljši rezultat`{:class="block3variables"}in v tem primeru uporabi `točke`{:class="block3variables"}, kot novo vrednost spremenljivke `najboljši rezultat`{:class="block3variables"}.

![Figura odra](images/stage-sprite.png)

```blocks3
    define preveri najboljši rezultat
	if <(točke :: variables) > (najboljši rezultat)> then
		set [najboljši rezultat v] to (točke :: variables)
	end
```

--- /task ---

--- task ---

Dodaj svoj novi blok v kodo odra v zaključek programa, pred koncem.

![Figura odra](images/stage-sprite.png)

```blocks3
when flag clicked
set [življenja v] to (3)
set [točke v] to (0)
wait until <(življenja) < (1)>
+ preveri najboljši rezultat :: custom
stop [all v]
```

--- /task ---

--- task ---

Dvakrat odigraj svojo igro, da vidiš ali se točke pravilno shranijo kot `najboljši rezultat`{:class="block3variables"}.

--- /task ---