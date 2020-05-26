## अंक हासिल करें या जीवन खो दें

अब आप कुछ डॉट्स जोड़ने जा रहे हैं जिन्हें खिलाड़ी को इकट्ठा करना है।

--- task ---

'red' नामक एक नया स्प्राइट बनाएँ। यह स्प्राइट एक छोटा लाल बिंदु होना चाहिए।

![लाल डॉट स्प्राइट](images/dots-red.png)

--- /task ---

--- task ---

हर कुछ सेकंड में स्प्राइट का एक नया क्लोन बनाने के लिए इस स्क्रिप्ट को अपने 'red' स्प्राइट में जोड़ें:

![लाल डॉट स्प्राइट](images/red-sprite.png)

```blocks3
    when flag clicked
    hide
    wait (2) seconds
    forever
        create clone of (myself v)
        wait (pick random (5) to (10)) secs
    end
```

--- /task ---

यदि आप अभी हरे झंडे पर क्लिक करते हैं, तो ऐसा लगता है कि कुछ नहीं हो रहा है। ऐसा इसलिए है क्योंकि क्लोन किए गए सभी स्प्राइट छिपे हुए हैं और वे एक ही स्थान पर दिखाई देंगे।

आप स्टेज के चार कोनों में से किसी एक कोने में नया क्लोन बनाने के लिए कोड जोड़ने जा रहे हैं।

![स्क्रीनशॉट](images/dots-start.png)

--- task ---

एक नई सूची बनाएं जिसे `आरंभ स्थान`{:class="block3variables"} कहा जाता है, सूची के `(+)` आइकन पर क्लिक करें और  `-180`{:class="block3variables"} और `180`{:class="block3variables"} मान जोड़ें I 

![लाल डॉट स्प्राइट](images/red-sprite.png)

![180 और -180 की सूची](images/dots-list.png)

[[[generic-scratch3-make-list]]]

तब आप इस बॉक्स को अचयनित करके सूची छिपा सकते हैं:

![सूची को छिपाएं](images/hide-list.png)

--- /task ---

ध्यान दें कि स्टेज के प्रत्येक कोने के लिए समन्वय `180` और `-180` का एक संयोजन है। इसका मतलब है कि आप सूची का उपयोग स्टेज के अनियमित कोने का चयन करने में कर सकते हैं।

--- task ---

इस कोड को 'डॉट' स्प्राइट में जोड़ें ताकि प्रत्येक नया स्प्राइट क्लोन एक अनियमित कोने में दिखाई दे और फिर धीरे-धीरे कंट्रोलर स्प्राइट की ओर बढ़े।

![लाल डॉट स्प्राइट](images/red-sprite.png)

```blocks3
    when I start as a clone
    go to x: (item (pick random (1) to (2)) of [start positions v]) y: (item (pick random (1) to (2)) of [start positions v])
    point towards (controller v)
    show
    repeat until <touching (controller v)?>
        move (1) steps
    end
```

--- /task ---

यह नया कोड या तो चुनता है `-180` या `180` एक्स और वाई पदों के लिए, जिसका अर्थ है कि प्रत्येक 'डॉट' स्प्राइट क्लोन स्टेज के एक कोने में शुरू होता है।

--- task ---

अपने प्रोजेक्ट का परीक्षण करें। आपको स्टेज के कोनों में लाल डॉट्स दिखाई देने चाहिए और धीरे-धीरे कंट्रोलर की ओर बढ़ते हैं।

![स्क्रीनशॉट](images/dots-red-test.png)

--- /task ---

--- task ---

`lives`{:class="block3variables"} और `score`{:class="block3variables"} नामक दो नए वेरिएबल्स बनाएं ।

![लाल डॉट स्प्राइट](images/red-sprite.png)

--- /task ---

--- task ---

खेल की शुरुआत में `lives`{:class="block3variables"} वेरिएबल में `3` और `score`{:class="block3variables"} में `0` सेट करने के लिए अपने स्टेज में कोड जोड़ें। 

![स्टेज स्प्राइट](images/stage-sprite.png)

```blocks3
when flag clicked
set [lives v] to (3)
set [score v] to (0)
```

--- /task ---

--- task ---

खिलाड़ी के अंतिम जीवन खोने पर खेल को समाप्त करने के लिए स्टेज की स्क्रिप्ट के अंत में इस कोड को जोड़ें:

![स्टेज स्प्राइट](images/stage-sprite.png)

```blocks3
    wait until <(lives :: variables) < [1]>
    stop [all v]
```

--- /task ---

खिलाड़ी को डॉट्स को पकड़ने के लिए अंक जीतने चाहिए, और डॉट्स को पकड़ने में विफल रहने के लिए जीवन खो देना चाहिए। एक डॉट तभी पकड़ा जा सकता है जब कंट्रोलर का कलर और डॉट का कलर समान हो।

--- task ---

स्प्राइट के अंत में कुछ कोड ब्लॉक जोड़ने के लिए 'red' डॉट स्प्राइट के स्क्रिप्स क्षेत्र पर वापस जाएं, `when I start as a clone`{:class="block3control"} स्क्रिप्ट।

सबसे पहले, डॉट क्लोन करें `5 कदम चलें`{:class="block3motion"} ताकि यह कंट्रोलर को ओवरलैप करे।

फिर कोड जोड़ें या तो `1` को `score`{:class="block3variables"} में जोड़ें यदि डॉट क्लोन का रंग छूने पर कंट्रोलर के रंग से मेल खाता है, या `1` को `lives`{:class="block3variables"} से घटा दे अगर उनका कलर मेल नहीं होता है।

[[[generic-scratch3-sound-from-library]]]

![लाल डॉट स्प्राइट](images/red-sprite.png)

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

--- /task ---

--- task ---

यह सुनिश्चित करने के लिए अपने खेल का परीक्षण करें कि:

1. यदि आप सही रंग के साथ डॉट से मेल नहीं खाते हैं तो आप एक जीवन खो देते हैं
2. आप एक अंक स्कोर कर लेंगे अगर आप एक बिंदु सही ढंग से मेल खाते हैं

--- /task ---