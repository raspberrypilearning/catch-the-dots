## التحدي: المزيد من النقاط 

الآن ستقوم برفع مستوى صعوبة اللعبة كلما نجح اللاعب في اللعب لوقت أطول. ستقوم بعمل ذلك عن طريق جعل النقاط تظهر بشكل أسرع و أسرع مع مرور الوقت.

\--- task \--- قم بإنشاء`متغير`{:class="block3variables"} باسم 'تأخير'.

![Stage sprite](images/stage-sprite.png) \--- /task \---

\--- task \--- اذهب إلى منطقة المقاطع البرمجية على مسرح العمل و أضف تعليمات برمجية جديدة تقوم بإعطاء المتغير `تأخير`{:class="block3variables"} القيمة `8` ثم بعد ذلك تقوم بخفض القيمة للمتغير `تأخير`{:class="block3variables"} خلال وقت استمرار اللعبة.

![Stage sprite](images/stage-sprite.png)

```blocks3
    عند نقر ⚑
اجعل [delay v] مساويًا (8)
كرِّر حتى <(delay) = (2)> 
  انتظر (10) ثانية
  غيِّر [delay v] بمقدار (-0.5)
end
```

\--- /task \---

لاحظ أن هذه التعليمات البرمجية تشبه بشكل كبير التعليمات البرمجية التي ستسخدمها في حال إنشائك لمؤقت عد تنازلي!

بعد ذلك, استخدم المتغير `تأخير`{:class="block3variables"} في التعليمات البرمجية الخاصة بالكائنات 'أحمر', 'أصفر', و 'أزرق'.

\--- task \--- Remove the code block that makes the game wait a random number of seconds between making the dot sprite clones. Replace the block you've removed with your new `delay`{:class="block3variables"} variable:

![لقطة الشاشة](images/all-dots.png)

```blocks3
<br />-   wait (pick random (5) to (10)) secs
    wait (delay :: variables) secs
```

Do this for all three dot sprites.

\--- /task \---

\--- task \--- Test the game, and check whether the dots begin to appear more quickly as the game goes on.

+ Does this work for all three coloured dots?
+ Can you see that the value of the `delay`{:class="block3variables"} variable decreases? \--- /task \---