## ಕಂಟ್ರೊಲ್ರ್ಅನ್ನು ರಚಿಸಿ

ಚುಕ್ಕೆಗಳನ್ನು ಸಂಗ್ರಹಿಸಲು ಆಟಗಾರನು ಬಳಸುವವನ್ನುಕಂಟ್ರೊಲ್ರ್ಅನ್ನು ರಚಿಸುವ ಮೂಲಕ ಪ್ರಾರಂಭಿಸಿ.

\--- task \---

'ಚುಕ್ಕೆಗಳನ್ನು ಹಿಡಿಯಿರಿ' scratch ಸ್ಟಾರ್ಟರ್ ಪ್ರಾಜೆಕ್ಟ್ ತೆರೆಯಿರಿ.

**Online:** open the starter project at [rpf.io/dots-on](https://rpf.io/dots-on){:target="_blank"}.

ನೀವು scratch ಖಾತೆಯನ್ನು ಹೊಂದಿದ್ದರೆ ಕ್ಲಿಕ್ ಮಾಡುವ ಮೂಲಕ ನೀವು ನಕಲನ್ನು ಮಾಡಬಹುದು **ರಿಮಿಕ್ಸ್**.

**Offline:** download the starter project from [rpf.io/p/en/catch-the-dots-go](https://rpf.io/p/en/catch-the-dots-go), and then open it in the Scratch offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff).

\--- /task \---

ನೀವು ಕಂಟ್ರೊಲ್ರ್ sprite ಅನ್ನು ನೋಡಬೇಕು:

![screenshot](images/dots-controller.png)

\--- task \---

ಆಟಗಾರನು right arrow key ಅನ್ನು ಒತ್ತಿದರೆ sprite right ತಿರುಗುವಂತೆ ನಿಯಂತ್ರಕ sprite ಗೆ ಕೆಲವು code ಸೇರಿಸಿ:

![ಕಂಟ್ರೊಲ್ರ್ sprite](images/controller-sprite.png)

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

ನಿಮ್ಮ ಕೋಡ್ಅನ್ನು ಪರೀಕ್ಷಿಸಿ. ನೀವು right arrow key ಅನ್ನು ಒತ್ತಿದಾಗ ಕಂಟ್ರೊಲ್ರ್ ಬಲಕ್ಕೆ ತಿರುಗಬೇಕು.

\--- /task \---

\--- task \---

ಕಂಟ್ರೊಲ್ರ್ sprite‌ಗೆ ಕೋಡ್ ಸೇರಿಸಿ sprite ಎಡಕ್ಕೆ ತಿರುಗುವಂತೆ ಮಾಡಲು left arrow key ಆಟಗಾರನು ಒತ್ತಿದರೆ.

![ಕಂಟ್ರೊಲ್ರ್ sprite](images/controller-sprite.png)

\--- hints \---

\--- hint \---

Right arrow key ಅನ್ನು ಒತ್ತಲಾಗಿದೆಯೇ ಮತ್ತು sprite right ತಿರುಗುತ್ತದೆಯೇ ಎಂದು ಪರಿಶೀಲಿಸುವ code ಅನ್ನು ಹುಡುಕಿ. ಈ code ‌ನ ನಕಲನ್ನು ನೀವು ಸೇರಿಸಬಹುದೇ ಮತ್ತು ನಕಲನ್ನು ಬದಲಾಯಿಸಬಹುದಾಗಿದ್ದು ಅದು left arrow key ಅನ್ನು ಒತ್ತಿದೆಯೆ ಎಂದು ಪರಿಶೀಲಿಸುತ್ತದೆ ಮತ್ತು sprite left ತಿರುಗುವಂತೆ ಮಾಡುತ್ತದೆ?

\--- /hint \---

\--- hint \---

ನಿಮಗೆ ಅಗತ್ಯವಿರುವ ಬ್ಲಾಕ್ ಗಳು ಇಲ್ಲಿವೆ:

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

\--- /hint \---

\--- hint \---

ನಿಮ್ಮ ಕೋಡ್ ಹೇಗಿರಬೇಕು ಎಂಬುದು ಇಲ್ಲಿದೆ:

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