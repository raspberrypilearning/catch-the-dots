## 增加难度

现在你要使这个游戏在玩家长时间玩后有更高的难度. 你可以使小点每次出现越来越快.

\--- task \--- 创建一个新的`变量`{:class="block3variables"} 叫做 'delay'.

![Stage sprite](images/stage-sprite.png) \--- /task \---

\--- task \--- 在舞台精灵区域并创建一个新的脚本设置`delay`{:class="block3variables"} 变量值为 `8` 并且 当游戏开始运行时缓慢减少 `delay`{:class="block3variables"} 变量的值.

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

注意这个代码与你曾经创建过的倒计时的代码非常相像!

接下来, 在红色,黄色,蓝色精灵代码中使用 `delay`{:class="block3variables"} 变量.

\--- task \--- 删除游戏中等待随机数秒克隆精灵的代码块. 用新的带有 `delay`{:class="block3variables"} 变量的代码块替换刚删除的代码部分:

![screenshot](images/all-dots.png)

```blocks3
<br />-   wait (pick random (5) to (10)) secs
    wait (delay :: variables) secs
```

对三个精灵都执行相同的操作.

\--- /task \---

\--- task \--- 测试游戏, 检查随着游戏的进行小点出现的频率是否越来越快.

+ 对三种颜色的小点工作都正常吗?
+ 你能看到 `delay`{:class="block3variables"} 变量值在减少吗? \--- /task \---