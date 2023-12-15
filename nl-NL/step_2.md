## Een controller maken

Begin met het maken van een controller die de speler gebruikt om stippen te verzamelen.

\--- task \---

Open het 'Vang de stippen' Scratch startproject.

**Online:** open the starter project at [rpf.io/dots-on](https://rpf.io/dots-on){:target="_blank"}.

Als je een Scratch-account hebt, kun je een kopie maken door op **Remix** te klikken.

**Offline:** download the starter project from [rpf.io/p/en/catch-the-dots-go](https://rpf.io/p/en/catch-the-dots-go), and then open it in the Scratch offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff).

\--- /task \---

Je zou een controller sprite moeten zien:

![schermafbeelding](images/dots-controller.png)

\--- task \---

Voeg wat code toe aan de controller sprite om de sprite naar rechts te laten draaien als de speler op de rechter pijltjestoets klikt:

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

\--- task \---

Test je code. De controller sprite zou naar rechts moeten draaien wanneer je op de rechter pijltjestoets drukt.

\--- /task \---

\--- task \---

Voeg code toe aan de controller sprite om de sprite naar links te laten draaien als de speler op de linker pijltjestoets klikt.

![Controller sprite](images/controller-sprite.png)

\--- hints \---

\--- hint \---

Zoek de code die controleert of de rechter pijltjestoets is ingedrukt en de sprite naar rechts doet draaien. Kun je een kopie van deze code toevoegen en de kopie aanpassen zodat deze controleert of de linker pijltjestoets is ingedrukt en de sprite naar links doet draaien?

\--- /hint \---

\--- hint \---

Dit zijn de blokken die je nodig hebt:

```blocks3
<toets (spatiebalk v) ingedrukt?>

draai (15) graden naar links

als <> dan

end
```

\--- /hint \---

\--- hint \---

Zo zou je code eruit moeten zien:

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

\--- /hint \---

\--- /hints \---

\--- /task \---