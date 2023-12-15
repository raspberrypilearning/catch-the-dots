## একটি নিয়ামক তৈরি করুন

কোনও নিয়ামক তৈরি করে শুরু করুন যা প্লেয়ার বিন্দু সংগ্রহ করতে ব্যবহার করবে।.

\--- task \---

'Catch the dots' স্ক্র্যাচ স্টার্টার প্রকল্পটি খুলুন।.

**Online:** open the starter project at [rpf.io/dots-on](https://rpf.io/dots-on){:target="_blank"}.

আপনার যদি স্ক্র্যাচ অ্যাকাউন্ট থাকে তবে আপনি **Remix**. ক্লিক করে একটি অনুলিপি তৈরি করতে পারেন।.

**Offline:** download the starter project from [rpf.io/p/en/catch-the-dots-go](https://rpf.io/p/en/catch-the-dots-go), and then open it in the Scratch offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff).

\--- /task \---

আপনি একটি নিয়ামক sprite দেখতে পাওয়া উচিত:

![screenshot](images/dots-controller.png)

\--- task \---

প্লেয়ার ডান arrow কী টিপলে স্প্রাইটকে ডানদিকে ফেরাতে নিয়ন্ত্রণকারী স্প্রাইটে কিছু code যুক্ত করুন:

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

\--- task \---

আপনার code পরীক্ষা করুন।. আপনি যখন ডান arrow কী টিপবেন, তখন নিয়ামকটি ডানদিকে ঘুরবে.

\--- /task \---

\--- task \---

প্লেয়ার বাম arrow কী টিপলে স্প্রাইটকে বাম দিকে বাঁকানোর জন্য নিয়ামক স্প্রাইটে code যুক্ত করুন।.

![Controller sprite](images/controller-sprite.png)

\--- hints \---

\--- hint \---

ডান arrow কী টিপছে কিনা এবং স্প্রাইটকে ডানদিকে পরিণত করে কিনা তা যাচাই করে এমন code টি সন্ধান করুন. আপনি কি এই code টির একটি অনুলিপি যুক্ত এবং অনুলিপিটি পরিবর্তন করতে পারেন যাতে এটি বাম arrow কী টিপলে স্প্রাইটটি বামদিকে বাঁক দেয় কিনা তা পরীক্ষা করে?

\--- /hint \---

\--- hint \---

আপনার যেগুলি ব্লকগুলি দরকার তা এখানে রয়েছে:

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

\--- /hint \---

\--- hint \---

এখানে আপনার code টি এইরকম দেখতে হওয়া উচিত:

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