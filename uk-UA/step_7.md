## Рекорд

Ти будеш зберігати рекорд гри, щоб гравці могли бачити свої успіхи.

\--- task \---

Створи нову змінну з іменем `рекорд`{:class="block3variables"}.

![спрайт Сцени](images/stage-sprite.png)

\--- /task \---

\--- task \---

Вибери Сцену. Клацни "Мої блоки" і створи новий власний блок з іменем `перевірка рекорду`{:class="block3myblocks"}.

![спрайт Сцени](images/stage-sprite.png)

![знімок екрана](images/dots-custom-1.png)

\--- /task \---

\--- task \---

Додай до свого блоку код, щоб він перевіряв, чи поточне значення `рахунку`{:class="block3variables"} більше за значення змінної `рекорд`{:class="block3variables"}, і якщо так, то зберігав `рахунок`{:class="block3variables"} як нове значення `рекорду`{:class="block3variables"}.

![спрайт Сцени](images/stage-sprite.png)

```blocks3
    define check high score
    if <(score :: variables) > (high score)> then
        set [high score v] to (score :: variables)
    end
```

\--- /task \---

\--- task \---

Додай новий власний блок до скрипта Сцени перед його кінцем.

![спрайт Сцени](images/stage-sprite.png)

```blocks3
when flag clicked
set [lives v] to (3)
set [score v] to (0)
wait until <(lives) < (1)>

+ check high score :: custom
stop [all v]
```

\--- /task \---

\--- task \---

Зіграй в свою гру двічі, щоб перевірити, чи твій рахунок коректно зберігається як `рекорд`{:class="block3variables"}.

\--- /task \---