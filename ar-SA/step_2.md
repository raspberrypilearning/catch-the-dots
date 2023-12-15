## إنشاء عجلة تحكم دوَّارة

ابدء بإنشاء عجلة تحكم يستخدمها اللاعب لجمع النقاط.

\--- task \---

افتح مشروع السكراتش Scratch الابتدائي 'اجمع النقاط'.

**Online:** open the starter project at [rpf.io/dots-on](https://rpf.io/dots-on){:target="_blank"}.

اذا كنت تملك حساب على منصة السكراتش (Scratch) فيمكنك عمل نسخة بالضغط على **Remix**.

**Offline:** download the starter project from [rpf.io/p/en/catch-the-dots-go](https://rpf.io/p/en/catch-the-dots-go), and then open it in the Scratch offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff).

\--- /task \---

ستشاهد كائن عجلة التحكم:

![لقطة الشاشة](images/dots-controller.png)

\--- task \---

أضف بعض التعليمات البرمجية لكائن عجلة التحكم لجعلها تدور باتجاه اليمين اذا قام اللاعب بالضغط على مفتاح السهم الأيمن:

![كائن عجلة التحكم](images/controller-sprite.png)

```blocks3
    عند نقر ⚑
كرر باستمرار 
  إذا <key (right arrow v) pressed?> 
    استدر ↻ (3) درجات
  end
end
```

\--- /task \---

\--- task \---

اختبر تعليماتك البرمجية. يفترض أن تدور عجلة التحكم باتجاه اليمين في حال ضغطت على زر السهم الأيمن.

\--- /task \---

\--- task \---

أضف بعض التعليمات البرمجية لكائن عجلة التحكم لجعلها تدور باتجاه اليسار اذا قام اللاعب بالضغط على مفتاح السهم الأيسر.

![كائن عجلة التحكم](images/controller-sprite.png)

\--- hints \---

\--- hint \---

ابحث عن التعليمة البرمجية التي تتحقق مما إذا كان زر السهم الأيمن مضغوطاً و يجعل كائن عجلة التحكم يستدير لليمين. هل يمكنك إضافة نسخة من هذه التعليمة البرمجية، بعد اجراء بعض التعديلات عليها بحيث تتحقق مما إذا كان زر السهم الأيسر مضغوطاً و بالتالي تستدير عجلة التحكم نحو اليسار؟

\--- /hint \---

\--- hint \---

إليك الكتل التي تحتاجها:

```blocks3
<key (space v) pressed?>

استدر ↺ (15) درجة

إذا <>
end
```

\--- /hint \---

\--- hint \---

و هذا ما يجب أن تبدو عليه التعليمات البرمجية الخاصة بك:

```blocks3
    عند نقر ⚑
كرِّر باستمرار 
  إذا <key (right arrow v) pressed?> 
    استدر ↻ (3) درجة
  end
  + إذا <key (left arrow v) pressed?> 
  +   استدر ↺ (3) درجة
  + end
end
```

\--- /hint \---

\--- hints/ \---

\--- /task \---