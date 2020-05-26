## उच्च स्कोर

आप खेल के उच्च स्कोर को सेव करने जा रहे हैं ताकि खिलाड़ी देख सकें कि वे कितना अच्छा कर रहे हैं।

--- task ---

एक नया वेरिएबल बनाएं `high score`{:class="block3variables"}.

![स्टेज स्प्राइट](images/stage-sprite.png)

--- /task ---

--- task ---

स्टेज का चयन करें। 'My blocks' पर क्लिक करें और एक नया कस्टम ब्लॉक `check high score` {:class="block3myblocks"} बनाएं I

![स्टेज स्प्राइट](images/stage-sprite.png)

![स्क्रीनशॉट](images/dots-custom-1.png)

--- /task ---

--- task ---

अपने कस्टम ब्लॉक में कोड जोड़ें ताकि ब्लॉक जाँच कर सके कि `score`{:class="block3variables"} का वर्तमान मान `high score`{:class="block3variables"} वेरिएबल के मान से अधिक है या नहीं और फिर `score`{:class="block3variables"} के मान को `high score`{:class="block3variables"} के नए मूल्य के रूप में सेव करें I

![स्टेज स्प्राइट](images/stage-sprite.png)

```blocks3
    define check high score
    if <(score :: variables) > (high score)> then
        set [high score v] to (score :: variables)
    end
```

--- /task ---

--- task ---

स्क्रिप्ट को अंत करने से पहले स्टेज स्क्रिप्ट में अपना नया कस्टम ब्लॉक जोड़ें।

![स्टेज स्प्राइट](images/stage-sprite.png)

```blocks3
when flag clicked
set [lives v] to (3)
set [score v] to (0)
wait until <(lives) < (1)>

+ check high score :: custom
stop [all v]
```

--- /task ---

--- task ---

अपना गेम दो बार खेलें ये देखने के लिए की आपका स्कोर ठीक तरीके से `high score`{:class="block3variables"} में सेव हो रहा है या नहीं।

--- /task ---