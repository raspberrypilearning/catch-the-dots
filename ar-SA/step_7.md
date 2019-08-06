## أعلى نتيجة

ستقوم بحفظ أعلى درجة تم تحقيقها، بحيث يمكن للاعب معرفة مدى تقدمه.

\--- task \--- قم بإنشاء متغير جديد يسمى `أعلى درجة`{:class="block3variables"}.

![Stage sprite](images/stage-sprite.png)

\---/task--

\--- task \--- اختر مسرح العمل. انقر على 'لبناتي' و أنشئ لبنة جديدة تسمى `التحقق من أعلى درجة`{:class="block3myblocks"}.

![Stage sprite](images/stage-sprite.png) ![لقطة الشاشة](images/dots-custom-1.png)

\--- /task \---

\--- task \--- أضف تعليمات برمجية إلى اللبنة الجديدة التي أنشئتها بحيث تقوم بالتحقق ما إذا كانت القيمة الحالية للمتغير`الدرجة`{:class="block3variables"} أكبر من قيمة المتغير `أعلى درجة`{:class="block3variables"}, ثم بعد ذلك تقوم بحفظ قيمة `الدرجة`{:class="block3variables"} كالقيمة الجديدة للمتغير `أعلى درجة`{:class="block3variables"}.

![Stage sprite](images/stage-sprite.png)

```blocks3
    عرِّف التحقق من أعلى درجة
إذا <(الدرجة :: variables) > (أعلى درجة)> 
  اجعل [أعلى درجة v] مساويًا (الدرجة :: variables)
end
```

\---/task\---

\--- task \--- أضف اللبنة الجديدة للمقاطع البرمجية على مسرح العمل قبل نهاية النص البرمجي.

![Stage sprite](images/stage-sprite.png)

```blocks3
when flag clicked
set [lives v] to (3)
set [score v] to (0)
wait until <(lives) < (1)>

+ check high score :: custom
stop [all v]
```

\--- /task \---

\--- task \---

Play your game twice to check whether your score gets correctly saved as the `high score`{:class="block3variables"}.

\--- /task \---