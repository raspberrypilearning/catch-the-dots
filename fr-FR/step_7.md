## Score élevé

Vous allez sauvegarder le meilleur score du jeu, afin que les joueurs puissent voir à quel point ils vont bien.

\--- task \--- Créez une nouvelle variable appelée `high score`{: class = "block3variables"}.

![Sprite de scène](images/stage-sprite.png)

\--- /tâche \---

\--- task \--- Sélectionnez la scène. Cliquez sur 'Mes blocs' et créez un nouveau bloc personnalisé appelé `check high score`{: class = "block3myblocks"}.

![Sprite de scène](images/stage-sprite.png) ![capture d'écran](images/dots-custom-1.png)

\--- /tâche \---

\--- task \--- Ajoutez du code à votre bloc personnalisé afin que le bloc vérifie si la valeur actuelle de `score`{: class = "block3variables"} est supérieure à la valeur du `score le plus élevé`{: class = "block3variables"} variable, puis stocke la valeur de `score`{: class = "block3variables"} en tant que nouvelle valeur de `score élevé`{: class = "block3variables"}.

![Sprite de scène](images/stage-sprite.png)

```blocks3
    définir vérifier score élevé
    si <(score :: variables) > (score élevé)> puis
        jeu [score élevé v] à (score :: variables)
    fin
```

\--- /tâche \---

\--- task \--- Ajoutez votre nouveau bloc personnalisé au script Stage avant la fin du script.

![Sprite de scène](images/stage-sprite.png)

```blocks3
lorsque le drapeau cliqué sur
set [vit v] à (3)
jeu [note v] à (0)
attente jusqu'à <(vie) < (1)>

+ vérifier score élevé :: personnalisée
arrêt [tout v]
```

\--- /tâche \---

\--- tâche \---

Jouez votre jeu deux fois pour vérifier si votre score est correctement enregistré en tant que `meilleur score`{: class = "block3variables"}.

\--- /tâche \---