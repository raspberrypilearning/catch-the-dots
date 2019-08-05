## جمع النقاط

\--- task \--- قم بمضاعفة كائن النقطة 'أحمر' مرتين، و أطلق على الكائنات الجديدة المسميات 'أصفر' و 'أزرق'.

![لقطة الشاشة](images/dots-more-dots.png) \--- /task \---

\--- task \--- غير مظهر الكائنات الجديدة بحيث يتناسب لون كلاً منهما مع اسمه: الكائن 'أصفر' لونه أصفر، و الكائن 'أزرق' لونه أزرق. \--- /task \---

\--- task \--- غيّر التعليمات البرمجية لكل كائن بحيث يصبح على اللاعب أن يطابق نسخ كائنات النقاط مع اللون المناسب على عجلة التحكم ليكسب نقاط.

![لقطة الشاشة](images/dots-all-test.png)

\--- hints \--- \--- hint \--- This is the code you need to find and alter for both new sprites:

![لقطة الشاشة](images/dots-more-dots.png)

```blocks3
    if <touching color [#FF0000]?> then
        change [score v] by (1)
        play sound (pop v)
        ...
    end
```

\--- /hint \--- \--- hint \--- This is how you need to change the code for the yellow sprite:

```blocks3
    if <touching color [#FFFF00]? :: +> then
        change [score v] by (1)
        play sound (pop v)
    end
```

This is how you need to change the code for the blue sprite:

```blocks3
    if <touching color [#0000FF]? :: +> then
        change [score v] by (1)
        play sound (pop v)
    end
```

\--- /hint \--- \--- /hints \--- \--- /task \---

If you play the game now, you can see that the dots sometimes get created one top of each other.

\--- task \--- Change the code for the 'yellow' dot sprite so that it waits four seconds after the flag is clicked before appearing.

![Yellow dot](images/yellow-sprite.png)

```blocks3
    when flag clicked
    hide
+   wait (4) seconds
```

![Blue dot](images/blue-sprite.png)

Then change the code for the 'blue' dot sprite so that it waits 6 seconds after the flag is clicked before appearing.

\--- /task \---