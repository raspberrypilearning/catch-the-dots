## अधिक ठिपके

\--- task \---

'red' डॉट स्प्राइटचे दोन प्रत बनवा आणि त्यांचे नाव 'yellow' आणि 'blue' ठेवा.

![screenshot](images/dots-more-dots.png)

\--- /task \---

\--- task \---

प्रत्येक नवीन स्प्राईटचा रंग बदला: 'yellow' स्प्राइट पिवळा असावा आणि 'blue' स्प्राइट निळा असावा.

\--- /task \---

\--- task \---

प्रत्येक स्प्राईटचा कोड बदला जेणेकरून गुण मिळवण्यासाठी खेळाडूला नियंत्रकावरील अचूक रंगात डॉट प्रत जुळवावे लागेल.

![screenshot](images/dots-all-test.png)

\--- hints \---

\--- hint \---

नवीन स्प्राईटसाठी कोडमध्ये हा बदल करावा लागेल:

![screenshot](images/dots-more-dots.png)

```blocks3
    if <touching color [#FF0000]?> then
        change [score v] by (1)
        play sound (pop v)
        ...
    end
```

\--- /hint \---

\--- hint \---

अशा प्रकारे आपल्याला पिवळ्या स्प्राइटसाठी कोड बदलावा लागेल:

```blocks3
    if <touching color [#FFFF00]? :: +> then
        change [score v] by (1)
        play sound (pop v)
    end
```

अशा प्रकारे आपल्याला निळ्या स्प्राइटसाठी कोड बदलावा लागेल:

```blocks3
    if <touching color [#0000FF]? :: +> then
        change [score v] by (1)
        play sound (pop v)
    end
```

\--- /hint \---

\--- /hints \---

\--- /task \---

If you play the game now, you can see that the dots sometimes get created on top of each other.

\--- task \---

'yellow'' डॉट स्प्राइटसाठी कोड बदला जेणेकरून ध्वज दिसण्यापूर्वी ते चार सेकंद थांबेल.

![Yellow dot](images/yellow-sprite.png)

```blocks3
    when flag clicked
    hide
+   wait (4) seconds
```

![Blue dot](images/blue-sprite.png)

'blue'' डॉट स्प्राइटसाठी कोड बदला जेणेकरून ध्वज दिसण्यापूर्वी ते 6 सेकंद थांबेल.

\--- /task \---