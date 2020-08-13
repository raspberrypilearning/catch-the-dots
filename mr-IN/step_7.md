## उच्च गुण

आपण गेमची उच्च धावसंख्या वाचवणार आहात जेणेकरुन खेळाडू ते किती चांगले काम करीत आहेत हे पाहू शकेल.

--- task ---

`high score`{:class="block3variables"} नावाचे एक नवीन चल तयार करा.

![Stage sprite](images/stage-sprite.png)

--- /task ---

--- task ---

स्टेज निवडा. 'My blocks' वर क्लिक करा आणि`check high score`{:class="block3myblocks"} नावाचा नवीन ब्लॉक तयार करा.

![Stage sprite](images/stage-sprite.png)

![screenshot](images/dots-custom-1.png)

--- /task ---

--- task ---

आताचा `score`{:class="block3variables"} चला जर `high score`{:class="block3variables"} चलापेक्षा जास्त असेल तर `score`{:class="block3variables"} चलाचे मूल्य `high score`{:class="block3variables"} चलामध्ये नक्कल करा.

![Stage sprite](images/stage-sprite.png)

```blocks3
    define check high score
    if <(score :: variables) > (high score)> then
        set [high score v] to (score :: variables)
    end
```

--- /task ---

--- task ---

स्क्रिप्टच्या समाप्तीपूर्वी आपला नवीन कस्टम ब्लॉक स्टेज स्क्रिप्टमध्ये जोडा.

![Stage sprite](images/stage-sprite.png)

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

आपले गुण `high score`{:class="block3variables"} मध्ये योग्यरित्या जतन झाला आहे की नाही हे तपासण्यासाठी गेम दोनदा खेळा.

--- /task ---