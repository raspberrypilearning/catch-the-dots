## कंट्रोलर बनाना

एक कंट्रोलर बनाकर शुरू करें जो खिलाड़ी डॉट्स को इकट्ठा करने के लिए उपयोग करेगा।

\--- task \---

'Catch the dots' Scratch स्टार्टर प्रोजेक्ट खोलें।

**ऑनलाइन:** [rpf.io/dots-on](http://rpf.io/dots-on){:target="_blank"} पर स्टार्टर प्रोजेक्ट खोलें I

यदि आपके पास एक Scratch अकाउंट है, तो आप ** Remix ** पर क्लिक करके कापी बना सकते हैं।

** ऑफ़लाइन: ** स्टार्टर प्रोजेक्ट को [ rpf.io/p/en/catch-the-dots-go ](http://rpf.io/p/en/catch-the-dots-go) से डाउनलोड करें और फिर इसे Scratch ऑफ़लाइन एडीटर में खोलें।

यदि आपको स्क्रैच ऑफ़लाइन एडीटर को डाउनलोड और इंस्टॉल करने की आवश्यकता है तो आप उसे [rpf.io/scratchoff](http://rpf.io/scratchoff) {:target="_blank"} पर पा सकते हैं।

\--- /task \---

आपको एक कंट्रोलर स्प्राइट दिखना चाहिए:

![स्क्रीनशॉट](images/dots-controller.png)

\--- task \---

यदि खिलाड़ी दाहिना एरो बटन दबाता है तो स्प्राइट को दाहिने तरफ मोड़ने के लिए कंट्रोलर स्प्राइट में कुछ कोड जोड़ें:

![कंट्रोलर स्प्राइट](images/controller-sprite.png)

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

अपने कोड का परीक्षण करें। जब आप दाईं एरो को दबाते हैं कंट्रोलर को दाईं ओर स्पिन करना चाहिए ।

\--- /task \---

\--- task \---

यदि खिलाड़ी बाएं एरो बटन दबाता है तो स्प्राइट को बाएं तरफ मोड़ने के लिए कंट्रोलर स्प्राइट में कुछ कोड जोड़ें:

![कंट्रोलर स्प्राइट](images/controller-sprite.png)

\--- hints \---

\--- hint \---

उस कोड को ढूंढें जो यह जांचता है कि क्या दाहिना एरो बटन दबाया गया है और स्प्राइट को दाहिने तरफ मोड़े। क्या आप इस कोड की एक कापी जोड़ सकते हैं और कापी को बदल सकते हैं ताकि यह जांच सके कि क्या बायाँ एरो बटन दबाने पर स्प्राइट बाएं ओर मुड़ता है या नहीं?

\--- /hint \---

\--- hint \---

यहाँ पर ब्लॉक्स हैं जिनकी आपको आवश्यकता होगी:

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

\--- /hint \---

\--- hint \---

आपका कोड कुछ इस तरह दिखेगा:

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