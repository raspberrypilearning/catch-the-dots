## Plus de points

--- task ---

Duplique deux fois ton sprite « rouge» et nomme les deux nouveaux sprites «jaune» et «bleu».

![capture d’écran](images/dots-more-dots.png)

--- /task ---

--- task ---

Change le costume de chaque nouveau sprite pour que ce soit la bonne couleur: le sprite «jaune» doit être jaune, et le sprite «bleu» doit être bleu.

--- /task ---

--- task ---

Change le code de chaque sprite de sorte que le joueur doit faire correspondre le clone point à la bonne couleur sur le contrôleur pour marquer des points.

![capture d'écran](images/dots-all-test.png)

--- hints ---


--- hint ---

Voici le code que tu dois rechercher et modifier pour les deux nouveaux sprites:

![capture d'écran](images/dots-more-dots.png)

```blocks3
    if <touching color [#FF0000]?> then
		change [score v] by (1)
		play sound (pop v)
        ...
	end
```

--- /hint ---

--- hint ---

Voici comment tu dois changer le code pour le sprite jaune:

```blocks3
    if <touching color [#FFFF00]? :: +> then
        change [score v] by (1)
        play sound (pop v)
	end
```

Voici comment tu dois changer le code pour le sprite bleu:

```blocks3
    if <touching color [#0000FF]? :: +> then
        change [score v] by (1)
        play sound (pop v)
	end
```

--- /hint ---

--- /hints ---

--- /task ---

Si tu joues au jeu maintenant, tu peux voir que les points sont parfois créés l'un de l'autre.

--- task ---

Change le code du sprite «jaune» pour qu'il attende quatre secondes après que le drapeau soit cliqué avant d'apparaître.

![Point jaune](images/yellow-sprite.png)

```blocks3
    when flag clicked
	hide
+	wait (4) seconds
```

![Point bleu](images/blue-sprite.png)

Puis change le code du sprite «bleu» pour qu'il attende 6 secondes après que le drapeau soit cliqué avant d'apparaître.

--- /task ---