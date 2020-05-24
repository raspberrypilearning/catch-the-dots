## Більше точок

\--- task \---

Продублюй двічі спрайт "червона точка" та назви два нових спрайти "жовта точка" і "синя точка".

![screenshot](images/dots-more-dots.png)

\--- /task \---

\--- task \---

Зміни образ кожного з нових спрайтів, щоб вони були правильного кольору: "жовта точка" має бути жовтою, а "синя точка" — синьою.

\--- /task \---

\--- task \---

Зміни код кожного зі спрайтів, щоб для заробляння очок гравець мав попадати клоном точки в правильний колір на контроллері.

![screenshot](images/dots-all-test.png)

\--- hints \---

\--- hint \---

Ось код, який тобі треба буде знайти і змінити в обох нових спрайтах:

![screenshot](images/dots-more-dots.png)

```blocks3
    if <touching color [#FF0000]?> then
        change [score v] by (1)
        play sound (pop v)
        ...
    end
```

\--- /hint \---

\--- hint \---

This is how you need to change the code for the yellow sprite:

```blocks3
    if <touching color [#FFFF00]? :: +> then
        change [score v] by (1)
        play sound (pop v)
    end
```

This is how you need to change the code for the blue sprite:

```blocks3
    if <touching color [#0000FF]? :: +> then
        change [score v] by (1)
        play sound (pop v)
    end
```

\--- /hint \---

\--- /hints \---

\--- /task \---

If you play the game now, you can see that the dots sometimes get created one top of each other.

\--- task \---

Change the code for the 'yellow' dot sprite so that it waits four seconds after the flag is clicked before appearing.

![Yellow dot](images/yellow-sprite.png)

```blocks3
    when flag clicked
    hide
+   wait (4) seconds
```

![Blue dot](images/blue-sprite.png)

Then change the code for the 'blue' dot sprite so that it waits 6 seconds after the flag is clicked before appearing.

\--- /task \---