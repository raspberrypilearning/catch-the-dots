## गुण मिळवा किंवा आपला जीव गमावा

आता आपण आवश्यक असलेले काही ठिपके जोडणार आहात.

\--- task \---

'red' नावाचा एक नवीन स्प्राइट तयार करा. हे स्प्राइट एक लहान लाल ठिपका असावा.

![Red dot sprite](images/dots-red.png)

\--- /task \---

\--- task \---

प्रत्येक स्क्रिप्टमध्ये स्प्राइटचा नवीन प्रत तयार करण्यासाठी हे स्क्रिप्ट आपल्या 'red' स्प्राइटमध्ये जोडा:

![Red dot sprite](images/red-sprite.png)

```blocks3
    when flag clicked
    hide
    wait (2) seconds
    forever
        create clone of (myself v)
        wait (pick random (5) to (10)) secs
    end
```

\--- /task \---

जर आपण आता हिरव्या ध्वज क्लिक केले तर असे दिसत आहे की काहीही झाले नाही. याचे कारण असे की सर्व प्रत केलेल्या स्प्राइट लपविल्या आहेत आणि ते एकाच ठिकाणी दिसतात.

प्रत्येक नवीन प्रत स्टेजच्या चार कोपऱ्यापैकी एकामध्ये दिसण्यासाठी आपण कोड जोडणार आहात.

![screenshot](images/dots-start.png)

\--- task \---

`start positions`{:class="block3variables"} नावाची एक नवीन यादी तयार करा, मूल्ये जोडण्यासाठी यादीच्या `(+)`चिन्हावर क्लिक करा `-180`{:class="block3variables"} आणि `180`{:class="block3variables"}.

![Red dot sprite](images/red-sprite.png)

![List of 180 and -180](images/dots-list.png)

[[[generic-scratch3-make-list]]]

नंतर आपण या बॉक्सची निवड रद्द करुन यादी लपवू शकता:

![Hide the list](images/hide-list.png)

\--- /task \---

प्रत्येक कोपऱ्यातील समन्वय `180` आणि `-180` चे संयोजन आहे. याचा अर्थ आपण कोणताही स्टेजचा कोपरा निवडण्यासाठी यादीचा वापर करू शकता.

\--- task \---

प्रत्येक नवीन स्प्राइट प्रत कोणताही कोपऱ्यात दिसण्यासाठी हा कोड 'dot' स्प्राइटमध्ये जोडा आणि नंतर हळू हळू नियंत्रक स्प्राइटच्या दिशेने जा.

![Red dot sprite](images/red-sprite.png)

```blocks3
    when I start as a clone
    go to x: (item (pick random (1) to (2)) of [start positions v]) y: (item (pick random (1) to (2)) of [start positions v])
    point towards (controller v)
    show
    repeat until <touching (controller v)?>
        move (1) steps
    end
```

\--- /task \---

हा नवीन कोड एकतर `-180` किंवा `180` निवडतो x आणि y पोझिशन्ससाठी, म्हणजे प्रत्येक 'dot' स्प्राइट प्रत स्टेजच्या कोपऱ्यात सुरू होतो.

\--- task \---

आपल्या कोडची चाचणी घ्या. आपल्याला स्टेजच्या कोपऱ्यात लाल ठिपके दिसले पाहिजेत आणि हळू हळू नियंत्रकाच्या दिशेने जावे.

![screenshot](images/dots-red-test.png)

\--- /task \---

\--- task \---

`lives`{:class="block3variables"} आणि `score`{:class="block3variables"} नावाचे दोन नवीन चल(variables) तयार करा.

![Red dot sprite](images/red-sprite.png)

\--- /task \---

\--- task \---

खेळाच्या सुरुवातीला `lives`{:class="block3variables"} चल `3` वर आणि `score`{:class="block3variables"} `0` वर सेट करण्यासाठी आपल्या स्टेजमध्ये कोड जोडा. ![Stage sprite](images/stage-sprite.png)

```blocks3
when flag clicked
set [lives v] to (3)
set [score v] to (0)
```

\--- /task \---

\--- task \---

जेव्हा खेळाडू शेवटच्या जीवनात हरला तेव्हा गेम समाप्त करण्यासाठी स्टेजच्या स्क्रिप्टच्या शेवटी हा कोड जोडा:

![Stage sprite](images/stage-sprite.png)

```blocks3
    wait until <(lives :: variables) < [1]>
    stop [all v]
```

\--- /task \---

खेळाडूंनी ठिपके पकडण्यासाठी गुण जिंकले पाहिजेत आणि ठिपके पकडण्यात अयशस्वी झाल्यामुळे त्याने प्राण गमावले पाहिजे. नियंत्रकच्या रंगास ठिपक्याच्या रंगाशी जुळवून ठिपके फक्त पकडले जाऊ शकतात.

\--- task \---

स्प्राइटच्या शेवटी काही कोड ब्लॉक जोडण्यासाठी 'रेड' डॉट स्प्राइटच्या स्क्रिप्ट्स क्षेत्राकडे परत जा `when I start as a clone`{:class="block3control"} स्क्रिप्ट.

प्रथम, ठिपक्यांची प्रतला बनवा `move 5 steps`{:class="block3motion"} जेणेकरून ते नियंत्रकाच्या वरती येतील.

जेव्हा ठिपक्यांचा रंग आणि नियंत्रकाचा रंग सारखा असेल तेव्हा `score`{:class="block3variables"} `1` ने वाढवा किंवा जर त्यांचे रंग जुळत नसतील तर `lives`{:class="block3variables"} `1` ने कमी करा.

[[[generic-scratch3-sound-from-library]]]

![Red dot sprite](images/red-sprite.png)

```blocks3
    move (5) steps
    if <touching color [#FF0000]?> then
        change [score v] by (1)
        play sound (pop v) until done
    else
        change [lives v] by (-1)
        play sound (Laser1 v) until done
    end
    delete this clone
```

\--- /task \---

\--- task \---

सुनिश्चित करण्यासाठी आपल्या खेळाची चाचणी घ्या:

1. आपण योग्य रंगासह ठिपका न जुळल्यास आपण आपले जीवन गमावाल
2. आपण ठिपका योग्यरित्या जुळल्यास गुण मिळत राहील

\--- /task \---