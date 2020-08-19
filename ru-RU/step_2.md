## Создай контроллер

Начни с создания контроллера, который игрок будет использовать, чтобы ловить точки.

--- task ---

Открой стартовый проект Scratch "Поймай точки".

**Онлайн:** открой стартовый проект по адресу [scratch.mit.edu/projects/418806322](https://scratch.mit.edu/projects/418806322){:target="_blank"}.

Если у тебя есть учётная запись в Scratch, то ты можешь сделать копию, нажав **Ремикс**.

**Оффлайн:** скачай стартовый проект с [rpf.io/p/ru-RU/catch-the-dots-go](http://rpf.io/p/ru-RU/catch-the-dots-go) и затем открой его с помощью оффлайн редактора Scratch.

Если тебе необходимо скачать и установить оффлайн редактор Scratch, то ты можешь найти его на [rpf.io/scratchoff](http://rpf.io/scratchoff).

--- /task ---

Ты увидишь спрайт контроллера:

![снимок экрана](images/dots-controller.png)

--- task ---

Добавь код в спрайт контроллера, чтобы заставить спрайт повернуть направо, если игрок нажимает клавишу со стрелкой вправо:

![Спрайт контроллера](images/controller-sprite.png)

```blocks3
    when flag clicked
	  forever
		  if <key (right arrow v) pressed?> then
			  turn right (3) degrees
		  end
	  end
```

--- /task ---

--- task ---

Проверь свой код. Контроллер должен вращаться вправо при нажатии клавиши со стрелкой вправо.

--- /task ---

--- task ---

Добавь код в спрайт контроллера, чтобы заставить спрайт повернуть налево, если игрок нажимает клавишу со стрелкой влево.

![Спрайт контроллера](images/controller-sprite.png)

--- hints ---


--- hint ---

Найди код, который проверяет, нажата ли клавиша со стрелкой вправо и заставляет спрайт поворачиваться направо. Можешь ли ты добавить копию этого кода и изменить ее так, чтобы она проверяла, нажата ли клавиша со стрелкой влево, и поворачивала бы спрайт влево?

--- /hint ---

--- hint ---

Вот блоки, которые тебе понадобятся:

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

--- /hint ---

--- hint ---

Вот как должен выглядеть твой код:

```blocks3
    when flag clicked
	  forever
		  if <key (right arrow v) pressed?> then
			  turn right (3) degrees
		  end
+ 		if <key (left arrow v) pressed?> then
			  turn left(3) degrees
		  end
	  end
```

--- /hint ---

--- /hints ---

--- /task ---