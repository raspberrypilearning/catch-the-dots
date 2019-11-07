## 更多小点

\--- task \--- 复制'red'小点精灵两次, 起名为'yellow'和'blue'.

![screenshot](images/dots-more-dots.png) \--- /task \---

\--- task \--- 修改每个新精灵的造型, 以便可以匹配正确的颜色:'yellow'精灵应该是黄色, 'blue'精灵应该是蓝色. \--- /task \---

\--- task \--- 修改每个精灵的代码, 以便玩家匹配正确的颜色获取得分.

![screenshot](images/dots-all-test.png)

\--- hints \--- \--- hint \--- 这是你需要在每个新精灵中找到和修改的代码:

![screenshot](images/dots-more-dots.png)

```blocks3
    if <touching color [#FF0000]?> then
        change [score v] by (1)
        play sound (pop v)
        ...
    end
```

\--- /hint \--- \--- hint \--- 这是你需要为黄色小点精灵修改的代码:

```blocks3
    if <touching color [#FFFF00]? :: +> then
        change [score v] by (1)
        play sound (pop v)
    end
```

这是你需要为蓝色精灵修改的代码:

```blocks3
    if <touching color [#0000FF]? :: +> then
        change [score v] by (1)
        play sound (pop v)
    end
```

\--- /hint \--- \--- /hints \--- \--- /task \---

如果你现在玩游戏, 你可以看到小点有时会创建在其他小点身上, 同时创建多个小点.

\--- task \--- 修改'yellow'小点精灵的代码以便在点击绿色旗帜后等待四秒再出现.

![Yellow dot](images/yellow-sprite.png)

```blocks3
    when flag clicked
    hide
+   wait (4) seconds
```

![Blue dot](images/blue-sprite.png)

然后修改'blue'小点精灵的代码以便在点击绿色旗帜后等待6秒才出现.

\--- /task \---