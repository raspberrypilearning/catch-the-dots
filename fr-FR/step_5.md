## Augmenter la difficulté

Maintenant, plus le joueur joue longtemps, plus le jeu est difficile. Pour ce faire, les points apparaissent de plus en plus rapidement au fil du temps.

--- task ---

Crée une nouvelle `variable`{:class="block3variables"} appelée «délai».

![Sprite Scène](images/stage-sprite.png)

--- /task ---

--- task ---

Va dans la zone des scripts de scène et crée un nouveau script qui définit la variable `délai`{:class="block3variables"} à `8` puis réduit lentement la valeur de `délai`{:class="block3variables"} pendant que le jeu s'exécute.

![Sprite Scène](images/stage-sprite.png)

```blocks3
    when flag clicked
	set [délai v] to (8)
	repeat until < (délai) = (2)>
		wait (10) seconds
		change [délai v] by (-0.5)
	end
```

--- /task ---

Note que ce code est très similaire au code que tu utiliseras pour créer un compte à rebours!

Ensuite, utilise la variable `délai`{:class="block3variables"} dans les scripts de code des sprites «rouge», «jaune» et «bleu».

--- task ---

Supprime le bloc de code qui fait attendre le jeu un nombre aléatoire de secondes entre la création des clones de sprite point. Remplace le bloc que tu as supprimé avec ta nouvelle variable `délai`{:class="block3variables"}:

![capture d'écran](images/all-dots.png)

```blocks3
-   attendre (nombre aléatoire entre (5) et (10)) secondes
    attendre (délai :: variables) secondes
```

Fais cela pour les trois sprites point.

--- /task ---

--- task ---

Teste le jeu et vérifie si les points commencent à apparaître plus rapidement au fur et à mesure que le jeu se poursuit.

+ Est-ce que cela fonctionne pour les trois points colorés?
+ Peux-tu voir que la valeur de la variable `délai`{:class="block3variables"} diminue?

--- /task ---