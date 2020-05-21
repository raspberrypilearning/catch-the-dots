## Gagner des points ou perdre des vies

Maintenant tu vas ajouter quelques points que le joueur doit collecter.

--- task ---

Crée un nouveau sprite appelé «rouge». Ce sprite doit être un petit point rouge.

![Sprite point rouge](images/dots-red.png)

--- /task ---

--- task ---

Ajoute ce script à ton sprite «rouge» pour créer un nouveau clone du sprite toutes les quelques secondes:

![Sprite point rouge](images/red-sprite.png)

```blocks3
    when flag clicked
    cacher
    attendre (2) secondes
    répéter indéfiniment
        créer un clone de (moi-même v)
        attendre (nombre aléatoire entre (5) et (10)) secondes
    fin
```

--- /task ---

Si tu cliques sur le drapeau vert maintenant, il semblerait que rien ne se produit. En effet, tous les sprites clonés sont cachés et apparaissent au même endroit.

Tu vas ajouter du code pour que chaque nouveau clone apparaisse dans l'un des quatre coins de la scène.

![capture d'écran](images/dots-start.png)

--- task ---

Crée une nouvelle liste appelée `positions de départ`{:class="block3variables"}, clique sur l'icône `(+)` de la liste pour ajouter les valeurs `-180`{:class="block3variables"} et `180`{:class="block3variables"}.

![Sprite point rouge](images/red-sprite.png)

![Liste de 180 et -180](images/dots-list.png)

[[[generic-scratch3-make-list]]]

Ensuite, tu peux cacher la liste en désélectionnant cette case:

![Cacher la liste](images/hide-list.png)

--- /task ---

Note que la coordonnée pour chaque coin de la scène est une combinaison de `180` et `-180`. Cela signifie que tu peux utiliser la liste pour choisir un coin de la scène au hasard.

--- task ---

Ajoute ce code au sprite « point » pour faire apparaître chaque nouveau clone de sprite dans un coin aléatoire et ensuite se diriger lentement vers le sprite du contrôleur.

![Sprite point rouge](images/red-sprite.png)

```blocks3
    quand je commence comme un clone
    aller à x: (élément (nombre aléatoire entre (1) et (2)) de [positions de départ v]) y: (élément (nombre aléatoire entre (1) et (2)) de [positions de départ v])
    s'orienter vers (contrôleur v)
    montrer
    repeat until <touching (contrôleur v)?>
		move (1) steps
	end
```

--- /task ---

Ce nouveau code choisit soit `-180` ou `180` pour les positions x et y, ce qui signifie que chaque clone de sprite «point» commence dans un coin de la scène.

--- task ---

Teste ton projet. Tu devrais voir apparaître des points rouges dans les coins de la scène et se déplacer lentement vers le contrôleur.

![capture d'écran](images/dots-red-test.png)

--- /task ---

--- task ---

Crée deux nouvelles variables appelées `vies`{:class="block3variables"} et `score`{:class="block3variables"}.

![Sprite point rouge](images/red-sprite.png)

--- /task ---

--- task ---

Ajoute du code à ta scène pour définir la variable `vies`{:class="block3variables"} à `3` et le `score`{:class="block3variables"} à `0` au début du jeu. 

![Sprite Scène](images/stage-sprite.png)

```blocks3
when flag clicked
set [vies v] to (3)
set [score v] to (0)
```

--- /task ---

--- task ---

Ajoute ce code à la fin du script de la scène pour que la partie se termine lorsque le joueur perd la dernière vie:

![Sprite Scène](images/stage-sprite.png)

```blocks3
    attendre jusqu'à ce que <(vies :: variables) < [1]>
    stop [tout v]
```

--- /task ---

Le joueur doit gagner des points pour avoir attrapé des points et doit perdre des vies pour ne pas avoir attrapé des points. Un point ne peut être attrapé qu'en associant la couleur du contrôleur à la couleur du point.

--- task ---

Retourne à la zone des scripts du sprite «rouge» pour ajouter des blocs de code à la fin du sprite `quand je commence comme un clone`{:class="block3control"}.

Tout d'abord, fais en sorte que le clone point se `déplace de 5 pas`{:class="block3motion"} pour qu'il chevauche le contrôleur.

Ajoute ensuite du code pour ajouter `1` à `score`{:class="block3variables"} si la couleur du clone point correspond à la couleur du contrôleur quand il touche, ou pour enlever `1` des `vies`{:class="block3variables"} si leurs couleurs ne correspondent pas.

[[[generic-scratch3-sound-from-library]]]

![Sprite point rouge](images/red-sprite.png)

```blocks3
    move (5) steps
	if <touching color [#FF0000]?> then
		change [score v] by (1)
		play sound (pop v) until done
	else
		change [vies v] by (-1)
		play sound (Laser1 v) until done
	end
	delete this clone
```

--- /task ---

--- task ---

Teste ton nouveau code pour t'assurer que:

1. Tu perds une vie si tu ne fais pas correspondre un point avec la couleur exacte
2. Tu marques un point si tu fais correspondre un point correctement

--- /task ---