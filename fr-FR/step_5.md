## Augmenter la difficulté

Maintenant, plus le joueur joue longtemps, plus le jeu est difficile. Pour ce faire, les points apparaissent de plus en plus rapidement.

\--- tâche \--- Créer une nouvelle `variable`{: class = "block3variables"} appelée 'délai'.

![Sprite de scène](images/stage-sprite.png) \--- /tâche \---

\--- task \--- Allez dans la zone Scripts de la scène et créez un nouveau script définissant la variable `delay`{: class = "block3variables"} sur `8` , puis réduisant lentement la valeur de `delay`{: class = "block3variables"} pendant l'exécution du jeu.

![Sprite de scène](images/stage-sprite.png)

```blocks3
    lorsque le drapeau est cliqué sur
    réglez [délai v] sur (8)
    répétition jusqu'à < (délai) = (2)>
        attente (10) secondes
        modification [délai v] de (-0,5)
    fin
```

\--- /tâche \---

Notez que ce code est très similaire au code que vous utiliseriez pour créer un compte à rebours!

Ensuite, utilisez la variable `delay`{: class = "block3variables"} dans les scripts de code des sprites "rouge", "jaune" et "bleu".

\--- task \--- Supprimez le bloc de code qui oblige le jeu à attendre un nombre aléatoire de secondes entre les clones de création d'image-objet. Remplacez le bloc que vous avez supprimé par votre nouvelle variable `delay`{: class = "block3variables"}:

![capture d'écran](images/all-dots.png)

```blocks3
<br />- wait (pick random (5) to (10)) secondes
    wait (delay :: variables) secondes
```

Faites cela pour les trois sprites.

\--- /tâche \---

\--- tâche \--- Testez le jeu et vérifiez si les points commencent à apparaître plus rapidement au cours du jeu.

+ Est-ce que cela fonctionne pour les trois points colorés?
+ Pouvez-vous voir que la valeur de la variable `delay`{: class = "block3variables"} diminue? \--- /tâche \---