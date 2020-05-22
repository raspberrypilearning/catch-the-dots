## Создай контроллер

Начни с создания контроллера, который игрок будет использовать, чтобы ловить точки.

\--- task \---

Открой стартовый проект Scratch "Поймай точки".

**Онлайн:** открой стартовый проект по адресу [rpf.io/dots-on](http://rpf.io/dots-on){:target="_blank"}.

Если у тебя есть учётная запись в Scratch, то ты можешь сделать копию, нажав **Ремикс**.

**Оффлайн:** скачай стартовый проект с [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go) и затем открой его с помощью оффлайн редактора Scratch.

Если тебе необходимо скачать и установить оффлайн редактор Scratch, то ты можешь найти его на [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /task \---

Ты увидишь спрайт контроллера:

![снимок экрана](images/dots-controller.png)

\--- task \---

Add some code to the controller sprite to make the sprite turn right if the player presses the right arrow key:

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

Test your code. The controller should spin to the right when you press the right arrow key.

\--- /task \---

\--- task \---

Add code to the controller sprite to make the sprite turn left if the player presses the left arrow key.

![Controller sprite](images/controller-sprite.png)

\--- hints \---

\--- hint \---

Find the code that checks whether the right arrow key is pressed and makes the sprite turn right. Can you add a copy of this code, and change the copy so it checks whether the left arrow key is pressed and makes the sprite turn left?

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