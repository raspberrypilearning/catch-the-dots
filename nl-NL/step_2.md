## Een controller maken

Begin met het maken van een controller die de speler gebruikt om stippen te verzamelen.

Open het 'Vang de stippen' Scratch starter project.

**Online**: open het online starter project op [rpf.io/dots-on](http://rpf.io/dots-on){:target="_ blank"}.

Als je een Scratch-account hebt, kun je een kopie maken door op **Remix** te klikken.

**Offline:** download het starter project op [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go){:target="_ blank"} en open het vervolgens met behulp van de Scratch offline editor.

Als je de Scratch offline editor wilt downloaden en installeren dan kan je die vinden op [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /task \---

Je zou een controllersprite moeten zien:

![screenshot](images/dots-controller.png)

\--- task \--- Voeg wat code toe aan de controllersprite om de sprite naar rechts te draaien als de speler de rechter pijljestoets indrukt:

![Controller sprite](images/controller-sprite.png)

```blocks3
    wanneer groene vlag wordt aangeklikt
herhaal 
  als <toets (pijltje rechts v) ingedrukt?> dan 
    draai (3) graden naar rechts :: control
  end :: control
end
```

\--- /task \---

\--- task \--- Test je code. De controllersprite zou naar rechts moeten draaien wanneer je op de rechter pijltjestoets drukt. \--- /task \---

\--- task \--- Voeg code toe aan de controllersprite om de sprite naar links te draaien als de speler de linker pijljestoets indrukt.

![Controller sprite](images/controller-sprite.png)

\--- hints \--- \--- hint \---

Vind de code die controleert of de rechter pijltjestoets is ingedrukt en de sprite naar rechts doet draaien. Kun je een kopie van deze code toevoegen en de kopie aanpassen zodat deze de controleert of de linker pijltjestoets is ingedrukt en de sprite naar links doet draaien?

\--- /hint \--- \--- hint \--- Hier zijn de blokken die je nodig hebt:

```blocks3
<toets (spatiebalk v) ingedrukt?>

draai (15) graden naar links

als <> dan

end
```

\--- / hint \--- \--- hint \--- Hier is hoe je blok eruit zou moeten zien:

```blocks3
    wanneer groene vlag wordt aangeklikt
herhaal 
	als <toets (pijltje rechts v) ingedrukt?> dan 
		draai (3) graden naar rechts
	end

+	als <toets (pijltje links v) ingedrukt?> dan 
		draai (3) graden naar links
	end
end
```

\--- /hint \--- \--- /hints \--- \--- /task \---