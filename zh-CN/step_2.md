## 创建一个控制器

从创建一个控制器开始, 玩家用来收集彩色小点

\--- 任务 \--- 打开'Catch the dots'Scratch 初始项目。

**在线：** 在 [rpf.io/dots-on](http://rpf.io/dots-on){:target =“_ blank”}打开初始项目。

如果您有Scratch帐户，可以单击 **改编**制作副本。

**离线：** 从 [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go) 下载初始项目，然后使用Scratch离线编辑器打开它。

如果您需要下载并安装Scratch离线编辑器，可以在[ rpf.io/scratchoff ](http://rpf.io/scratchoff)中获取。

\--- /task \---

你会看到一个控制器精灵:

![screenshot](images/dots-controller.png)

\--- task \--- 在控制器精灵中增加一些代码, 如果玩家按右键, 控制器会向右旋转:

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

\--- task \--- 测试你的代码。 当你按键盘的右键时, 控制器应该向右旋转. \--- /task \---

\--- task \--- 在控制器精灵中增加一些代码, 如果玩家按左键, 控制器会向左旋转.

![Controller sprite](images/controller-sprite.png)

\--- hints \--- \--- hint \---

查看代码, 检查是否有当键盘右键按下并让精灵向右转动. 你能加入这段代码的拷贝, 并且修改这个拷贝检查是否键盘左键按下时精灵向左旋转?

\--- /hint \--- \--- hint \--- 以下是您需要的代码块：

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

\--- /hint \--- \--- hint \--- 你的代码应该是这个样子：

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

\--- /hint \--- \--- /hints \--- \--- /task \---