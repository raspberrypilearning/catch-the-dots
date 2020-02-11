## Création d'un contrôleur

Commence par créer un contrôleur que le joueur utilisera pour collecter des points.

\--- task \---

Ouvre le projet Scratch de démarrage « Attrape les points ».

**En ligne:** ouvre le projet de démarrage à [rpf.io/dots-on](http://rpf.io/dots-on){:target="_ blank"}.

Si tu as un compte Scratch, tu peux en créer une copie en cliquant sur **Remix**.

**Hors ligne:** télécharge le projet de démarrage à partir de [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go), puis ouvre-le à l'aide de l'éditeur Scratch hors-ligne.

Si tu veux télécharger et installer l’éditeur Scratch hors-ligne, tu peux le trouver ici : [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /task \---

Tu devrais voir un sprite contrôleur :

![capture d'écran](images/dots-controller.png)

\--- task \---

Ajoute du code au sprite du contrôleur pour le faire tourner à droite si le joueur appuie sur la touche fléchée droite :

![Sprite du contrôleur](images/controller-sprite.png)

```blocks3
    quand le drapeau est cliqué
    répéter indéfiniment
        si <key (right arrow v) pressed?> alors
            tourner à droite de (3) degrés
        fin
    fin
```

\--- /task \---

\--- task \---

Teste ton code. Le contrôleur devrait tourner vers la droite lorsque tu appuies sur la touche fléchée droite.

\--- /task \---

\--- task \---

Ajoute du code au sprite du contrôleur pour le faire tourner à gauche si le joueur appuie sur la touche fléchée gauche.

![Sprite du contrôleur](images/controller-sprite.png)

\--- hints \---

\--- hint \---

Trouve le code qui vérifie si la touche fléchée droite est appuyée et fait tourner le sprite à droite. Peux-tu ajouter une copie de ce code, et changer la copie pour qu'il vérifie si la touche fléchée gauche est appuyée et fait tourner le sprite à gauche ?

\--- /hint \---

\--- hint \---

Voici les blocs dont tu as besoin :

```blocks3
<key (space v) pressed?>

tourner à gauche de (15) degrés

si <> alors

fin
```

\--- /hint \---

\--- hint \---

Voici à quoi ton code devrait ressembler :

```blocks3
    quand le drapeau vert est cliqué
    répéter indéfiniment
        si <key (right arrow v) pressed?> alors
            tourner à droite de (3) degrés
        fin

+ si <key (left arrow v) pressed?> alors
            tourner à gauche de(3) degrés
        fin
    fin
```

\--- /hint \---

\--- /hints \---

\--- /task \---