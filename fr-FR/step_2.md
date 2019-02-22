## Créer un contrôleur

Commencez par créer un contrôleur que le joueur utilisera pour collecter des points.

\--- task \--- Ouvrez le projet de démarrage Scratch 'Catch the dots'.

**En ligne:** ouvrez le projet de démarrage à [rpf.io/dots-on](http://rpf.io/dots-on){: target = "_ blank"}. Si vous avez un compte Scratch, vous pouvez cliquer sur **Remix** dans le coin supérieur droit pour enregistrer une copie du projet.

**Hors ligne:** téléchargez le projet de démarrage à partir de [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go), puis ouvrez-le dans l'éditeur hors ligne Scratch.

Si vous devez télécharger et installer l'éditeur hors ligne Scratch, vous pouvez le trouver à l'adresse [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /tâche \---

Vous devriez voir un sprite de contrôleur:

![capture d'écran](images/dots-controller.png)

\--- task \--- Ajoutez du code au sprite du contrôleur pour le faire tourner à droite si le joueur appuie sur la flèche droite:

![Contrôleur sprite](images/controller-sprite.png)

```blocks3
    quand le drapeau a cliqué
    pour toujours
        si <key (right arrow v) pressed?> puis
            tourner à droite (3) degrés
        fin
    fin
```

\--- /tâche \---

\--- tâche \--- Testez votre code. Le contrôleur doit tourner à droite lorsque vous appuyez sur la touche fléchée droite. \--- /tâche \---

\--- task \--- Ajoutez du code à l'image-objet du contrôleur pour que celui-ci tourne à gauche si le joueur appuie sur la flèche gauche.

![Contrôleur sprite](images/controller-sprite.png)

\--- astuces \--- \--- astuces \---

Recherchez le code qui vérifie si la flèche droite est enfoncée et fait tourner le sprite à droite. Pouvez-vous ajouter une copie de ce code et modifier la copie afin qu'elle vérifie si la touche flèche gauche est enfoncée et fait tourner l'image-objet à gauche?

\--- / indice \--- \--- indice \--- Voici les blocs dont vous avez besoin:

```blocks3
<key (space v) pressed?>

tourner à gauche (15) degrés

si <> puis

fin
```

\--- / hint \--- \--- hint \--- Voici à quoi devrait ressembler votre code:

```blocks3
    lorsque l' indicateur cliqué
    pour toujours
        si <key (right arrow v) pressed?> puis
            , tourner à droite (3) degrés
        extrémité

+ si <key (left arrow v) pressed?> puis
            virage à gauche (3) degrés
        extrémité
    extrémité
```

\--- / astuce \--- \--- / astuces \--- \--- / tâche \---