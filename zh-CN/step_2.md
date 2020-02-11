## 创建一个控制器

首先创建一个控制器，玩家将使用该控制器来收集点。

\--- task \---

Open the 'Catch the dots' Scratch starter project.

**在线：** 在 [rpf.io/dots-on](http://rpf.io/dots-on){:target =“_ blank”}打开初始项目。

如果您有一个Scratch帐户，您可以通过点击**Remix**复制。

**离线：** 从 [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go) 下载初始项目，然后使用Scratch离线编辑器打开它。

如果您需要下载并安装Scratch离线编辑器，可以在[ rpf.io/scratchoff ](http://rpf.io/scratchoff)中获取。

\--- /task \---

你会看到一个控制器精灵:

![截屏](images/dots-controller.png)

\--- task \---

Add some code to the controller sprite to make the sprite turn right if the player presses the right arrow key:

![控制器精灵](images/controller-sprite.png)

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

测试你的代码。 当您按向右箭头键时，控制器应向右旋转。

\--- /task \---

\--- task \---

Add code to the controller sprite to make the sprite turn left if the player presses the left arrow key.

![控制器精灵](images/controller-sprite.png)

\--- hints \---

\--- hint \---

查看代码, 检查是否有当键盘右键按下使精灵向右转动. 你能加入这段代码的拷贝, 并且修改这个拷贝检查是否键盘左键按下时精灵向左旋转?

\--- /hint \---

\--- hint \---

以下是你需要的代码：

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

\--- /hint \---

\--- hint \---

您的代码看起来应该是这样的：

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