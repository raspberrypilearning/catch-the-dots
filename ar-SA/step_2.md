## إنشاء قرص دوَّار

ابدء بإنشاء قرص تحكم يستخدمه اللاعب لجمع النقاط.

\--- task \--- افتح مشروع Scratch المبدئي 'اجمع النقاط'.

**بالاتصال بالانترنت**: افتح المشروع المبدئي من هنا [rpf.io/dots-on](http://rpf.io/dots-on){:target="_blank"}.

اذا كنت تملك حساب على منصة سكراتش (Scratch) فيمكنك عمل نسخة بالنقر على **Remix**.

**بدون اتصال انترنت** حمّل المشروع المبدئي من [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go){:target="_blank"} ثم اقتحه باستخدام محرر Scratch بدون اتصال انترنت.

لتنزيل و تركيب محرر Scratch على جهازك الشخصي, يمكنك الحصول عليه من هنا [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /task \---

يجب أن تشاهد كائن المتحكم:

![screenshot](images/dots-controller.png)

\--- task \--- أضف بعض التعليمات البرمجية لكائن قرص التحكم لجعله يدور باتجاه اليمين اذا قام اللاعب بالضغط على مفتاح السهم اليمين:

![Controller sprite](images/controller-sprite.png)

```blocks3
    عند نقر ⚑
كرر باستمرار 
  إذا <key (right arrow v) pressed?> 
    استدر ↻ (3) درجات
  end
end
```

\--- /task \---

\--- task \--- Test your code. The controller should spin to the right when you press the right arrow key. \--- /task \---

\--- task \--- Add code to the controller sprite to make the sprite turn left if the player presses the left arrow key.

![Controller sprite](images/controller-sprite.png)

\--- hints \--- \--- hint \---

Find the code that checks whether the right arrow key is pressed and makes the sprite turn right. Can you add a copy of this code, and change the copy so it checks whether the left arrow key is pressed and makes the sprite turn left?

\--- /hint \--- \--- hint \--- Here are the blocks you need:

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

\--- /hint \--- \--- hint \--- Here is what your code should look like:

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