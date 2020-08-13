## एक नियंत्रक तयार करा

ठिपके गोळा करण्यासाठी खेळाडू वापरेल असा नियंत्रक तयार करायला सुरूवात करा.

--- task ---

'Catch the dots' Scratch स्टार्टर प्रकल्प उघडा.

**ऑनलाइन:** स्टार्टर प्रकल्प [rpf.io/dots-on वर उघडा](http://rpf.io/dots-on){:target="_blank"}.

आपल्याकडे Scratch खाते असल्यास आपण **Remix** क्लिक करून एक नक्कल तयार करू शकता.

**ऑफलाइनः** स्टार्टर प्रकल्प [rpf.io/p/mr-IN/catch-the-dots-go वरून डाउनलोड करा](http://rpf.io/p/mr-IN/catch-the-dots-go), आणि नंतर ते Scratch ऑफलाइन संपादकात उघडा.

आपल्याला Scratch ऑफलाइन संपादक डाउनलोड आणि स्थापित करणे आवश्यक असल्यास, आपण ते [rpf.io/scratchoff](http://rpf.io/scratchoff) येथे शोधू शकता.

--- /task ---

आपण एक नियंत्रक स्प्राइट पहावा:

![screenshot](images/dots-controller.png)

--- task ---

जर खेळाडूने उजवीकडील बाण बटण दाबल तर स्प्राइटला उजवीकडे वळविण्यासाठी नियंत्रक स्प्राइटमध्ये काही कोड जोडा:

![Controller sprite](images/controller-sprite.png)

```blocks3
    when flag clicked
    forever
        if <key (right arrow v) pressed?> then
            turn right (3) degrees
        end
    end
```

--- /task ---

--- task ---

आपल्या कोडची चाचणी घ्या. आपण उजव बाण बटण दाबल्यास नियंत्रक उजवीकडे फिरले पाहिजे.

--- /task ---

--- task ---

जर खेळाडूने डावीकडील बाण बटण दाबल तर स्प्राइटला डावीकडे वळविण्यासाठी नियंत्रक स्प्राइटमध्ये काही कोड जोडा.

![Controller sprite](images/controller-sprite.png)

--- hints ---


--- hint ---

उजव बाण बटण दाबल आहे कि नाही हे तपासून स्प्राइटला उजवीकडे वळवणारा कोड शोधा. आपण या कोडची एक प्रत जोडू शकता आणि प्रत बदलू शकता जेणेकरून ती डावीकडील बाण बटण दाबल आहे की नाही हे तपासते आणि स्प्राइट डावीकडे वळवते?

--- /hint ---

--- hint ---

आपल्याला आवश्यक असलेले ब्लॉक येथे आहेत:

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

--- /hint ---

--- hint ---

आपला कोड कसा दिसला पाहिजे ते येथे आहे:

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

--- /hint ---

--- /hints ---

--- /task ---