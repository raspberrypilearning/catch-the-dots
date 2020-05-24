## Створи контроллер

Розпочни зі створення контроллера, яким гравець буде ловити точки.

\--- task \---

Відкрий початковий проєкт "Лови точки" у Скретч.

**Онлайн:** відкрий стартовий проєкт на [rpf.io/dots-on](http://rpf.io/dots-on){:target="_blank"}.

Якщо у тебе є обліковий запис Скретч, то ти можеш зробити копію проєкту, натиснувши **Ремікс**.

**Офлайн:** завантаж стартовий проект з [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go), а потім відкрий його за допомогою офлайн-редактора Scratch.

Якщо тобі треба завантажити та встановити офлайн-редактор Скретч, то ти можеш його знайти на [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /task \---

Ти маєш побачити спрайт контроллера:

![screenshot](images/dots-controller.png)

\--- task \---

Додай код до спрайта контроллера, щоб він повертався вправо кожного разу, коли гравець натискає клавішу зі стрілкою вправо:

![Controller sprite](images/controller-sprite.png)

```blocks3
    when flag clicked
    forever
        if <key (right arrow v) pressed?> then
            turn right (3) degrees
        end
    end
```

\--- /task \---

\--- task \---

Протестуй свій код. Контроллер має обератися вправо, коли ти натискаєш на клавішу зі стрілкою вправо.

\--- /task \---

\--- task \---

Додай код до контроллера, щоб обертати спрайт вліво, коли гравець натискає на клавішу зі стрілкою вліво.

![Controller sprite](images/controller-sprite.png)

\--- hints \---

\--- hint \---

Знайди код, який перевіряє, що натискається клавіша стрілки вправо, і повертає спрайт вправо. Can you add a copy of this code, and change the copy so it checks whether the left arrow key is pressed and makes the sprite turn left?

\--- /hint \---

\--- hint \---

Here are the blocks you need:

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

\--- /hint \---

\--- hint \---

Here is what your code should look like:

```blocks3
    when flag clicked
    forever
        if <key (right arrow v) pressed?> then
            turn right (3) degrees
        end

+       if <key (left arrow v) pressed?> then
            turn left(3) degrees
        end
    end
```

\--- /hint \---

\--- /hints \---

\--- /task \---