## Plus de points

\--- task \--- Dupliquez deux fois votre sprite 'point rouge' et nommez les deux nouveaux sprites 'jaune' et 'bleu'.

![capture d'écran](images/dots-more-dots.png) \--- /tâche \---

\--- tâche \--- Modifiez le costume de chaque nouveau sprite afin qu'il corresponde bien à la couleur: le sprite 'jaune' doit être jaune et le sprite 'bleu' doit être bleu. \--- /tâche \---

\--- task \--- Modifiez le code de chaque image-objet de sorte que le joueur doit faire correspondre le clone de points à la couleur correcte sur le contrôleur pour marquer des points.

![capture d'écran](images/dots-all-test.png)

\--- astuces \--- \--- astuce \--- Il s'agit du code que vous devez rechercher et modifier pour les deux nouveaux sprites:

![capture d'écran](images/dots-more-dots.png)

```blocks3
    si <touching color [#FF0000]?> alors
        changement [score v] de (1)
        joue le son (pop v)
...
    fin
```

\--- / hint \--- \--- hint \--- Voici comment modifier le code du sprite jaune:

```blocks3
    si <touche la couleur [# FFFF00]? :: +> puis
        changement [score v] de (1)
        jouer le son (pop v)
    fin
```

Voici comment modifier le code du sprite bleu:

```blocks3
    si <touche la couleur [# 0000FF]? :: +> puis
        changement [score v] de (1)
        jouer le son (pop v)
    fin
```

\--- / astuce \--- \--- / astuces \--- \--- / tâche \---

Si vous jouez au jeu maintenant, vous pouvez voir que les points sont parfois superposés.

\--- task \--- Modifiez le code de l'image-objet à points «jaune» afin qu'elle attende quatre secondes après le clic sur l'indicateur avant d'apparaître.

![Point jaune](images/yellow-sprite.png)

```blocks3
    lorsque le drapeau est cliqué
    masquer
+ attendre (4) secondes
```

![Point bleu](images/blue-sprite.png)

Ensuite, changez le code de l’image-objet «bleue» afin qu’elle attende 6 secondes après le clic sur le drapeau avant de paraître.

\--- /tâche \---