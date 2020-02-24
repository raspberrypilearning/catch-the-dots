## 增加难度

现在，随着玩家玩的时间越长，您将使游戏变得更加困难。 你可以使小点每次出现越来越快.

\--- task \---

Create a new `variable`{:class="block3variables"} called 'delay'.

![Stage sprite](images/stage-sprite.png)

\--- /task \---

\--- task \---

Go to the Stage's Scripts area and create a new script that sets the `delay`{:class="block3variables"} variable to `8` and then slowly reduces the value of `delay`{:class="block3variables"} while the game runs.

![Stage sprite](images/stage-sprite.png)

```blocks3
    when flag clicked
    set [delay v] to (8)
    repeat until < (delay) = (2)>
        wait (10) seconds
        change [delay v] by (-0.5)
    end
```

\--- /task \---

请注意，此代码与创建倒数计时器所使用的代码非常相似！

接下来, 在红色,黄色,蓝色精灵代码中使用 `delay`{:class="block3variables"} 变量.

\--- task \---

Remove the code block that makes the game wait a random number of seconds between making the dot sprite clones. 用新的带有 `delay`{:class="block3variables"} 变量的代码块替换刚删除的代码部分:

![截屏](images/all-dots.png)

```blocks3
<br />-   wait (pick random (5) to (10)) secs
    wait (delay :: variables) secs
```

对三个精灵都执行相同的操作.

\--- /task \---

\--- task \---

Test the game, and check whether the dots begin to appear more quickly as the game goes on.

+ 对三种颜色的小点工作都正常吗?
+ 你能看到 `delay`{:class="block3variables"} 变量值在减少吗?

\--- /task \---