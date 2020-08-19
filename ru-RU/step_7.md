## Рекорд

Теперь мы сохраним рекорд игры, чтобы игроки могли оценить свои успехи.

--- task ---

Создай новую переменную с именем `рекорд`{:class="block3variables"}.

![Спрайт Сцены](images/stage-sprite.png)

--- /task ---

--- task ---

Выбери Сцену. Перейди в «Другие блоки» и создай новый пользовательский блок с именем `проверь рекорд`{:class="block3myblocks"}.

![Спрайт Сцены](images/stage-sprite.png)

![снимок экрана](images/dots-custom-1.png)

--- /task ---

--- task ---

Добавь код в свой пользовательский блок так, чтобы блок проверял, является ли текущее значение `счёта`{:class="block3variables"} больше значения переменной `рекорд`{:class="block3variables"}, а затем сохраняет значение `счёта`{:class="block3variables"} в переменной `рекорд`{:class="block3variables"}.

![Спрайт Сцены](images/stage-sprite.png)

```blocks3
    define проверь рекорд
    if <(счёт :: variables) > (рекорд)> then
        set [рекорд v] to (счёт :: variables)
    end
```

--- /task ---

--- task ---

Добавь свой новый пользовательский блок в конец скрипта Сцены.

![Спрайт Сцены](images/stage-sprite.png)

```blocks3
when flag clicked
set [жизни v] to (3)
set [счёт v] to (0)
wait until <(жизни) < (1)>
+ проверь рекорд :: custom
stop [all v]
```

--- /task ---

--- task ---

Сыграй в игру дважды, чтобы проверить, правильно ли сохраняется счёт, как `рекорд`{:class="block3variables"}.

--- /task ---