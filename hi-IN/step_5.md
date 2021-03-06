## कठिनाई बढ़ाओ

अब आप खेल को और अधिक कठिन बनाने जा रहे हैं उस खिलाड़ी के लिए जो इसे अधिक समय तक खेलता है I आप ऐसा करेंगे कि डॉट्स समय के साथ और तेज गति से चलते दिखाई देंगे।

--- task ---

एक नया `वेरिएबल`{:class="block3variables"} बनाएं जिसे 'delay' कहा जाता है।

![स्टेज स्प्राइट](images/stage-sprite.png)

--- /task ---

--- task ---

स्टेज के स्क्रिप्ट्स के क्षेत्र में जाएं और एक नई स्क्रिप्ट बनाएं जो `delay`{:class="block3variables"} वेरिएबल सेट करता है `8` से और फिर धीरे-धीरे `delay`{:class="block3variables"} के मूल्य को कम करता है जब तक गेम चलता है।

![स्टेज स्प्राइट](images/stage-sprite.png)

```blocks3
    when flag clicked
    set [delay v] to (8)
    repeat until < (delay) = (2)>
        wait (10) seconds
        change [delay v] by (-0.5)
    end
```

--- /task ---

ध्यान दें कि यह कोड उस कोड के समान है जो आप एक काउंटडाउन टाइमर बनाने के लिए उपयोग करेंगे!

अगला, `delay`{:class="block3variables"} वेरिएबल का उपयोग 'red', 'yellow' और 'blue' स्प्राइट के कोड स्क्रिप्ट में करें।

--- task ---

उस कोड ब्लॉक को निकालें जो गेम को डॉट स्प्राइट क्लोन बनाने के बीच कुछ सेकंड की एक अनियमित संख्या की प्रतीक्षा करता है। आपके द्वारा हटाए गए ब्लॉक को अपने नए `delay`{:class="block3variables"} वेरिएबल से बदलें:

![स्क्रीनशॉट](images/all-dots.png)

```blocks3
-   wait (pick random (5) to (10)) secs
    wait (delay :: variables) secs
```

ऐसा तीनों डॉट स्प्राइट के लिए करें।

--- /task ---

--- task ---

खेल का परीक्षण करें और जाँच करें कि क्या खेल शुरू होते ही समय के साथ डॉट्स अधिक तेज़ी से दिखाई देने लगते हैं।

+ क्या यह तीनों रंगीन डॉट्स के लिए काम करता है?
+ क्या आप देख सकते हैं कि `delay`{:class="block3variables"} वेरिएबल का मूल्य घटता है?

--- /task ---