## High score (ಹೆಚ್ಚಿನ ಅಂಕ)

ನೀವು ಆಟದ high score ಅನ್ನು ಉಳಿಸಲಿದ್ದೀರಿ, ಇದರಿಂದ ಆಟಗಾರರು ಎಷ್ಟು ಚೆನ್ನಾಗಿ ಕಾರ್ಯನಿರ್ವಹಿಸುತ್ತಿದ್ದಾರೆ ಎಂಬುದನ್ನು ನೋಡಬಹುದು.

--- task ---

ಹೊಸ ವೇರಿಯೇಬಲ್ ಅನ್ನು ರಚಿಸಿ `high score`{:class="block3variables"}.

![ಹಂತ(Stage) sprite](images/stage-sprite.png)

--- /task ---

--- task ---

ಹಂತ ಆಯ್ಕೆಮಾಡಿ. ಕ್ಲಿಕ್ ಮಾಡಿ 'My blocks' ಮತ್ತು ಹೊಸದನ್ನು ರಚಿಸಿ custom ಬ್ಲಾಕ್ `check high score`{:class="block3myblocks"}.

![ಹಂತ sprite](images/stage-sprite.png)

![screenshot](images/dots-custom-1.png)

--- /task ---

--- task ---

ನಿಮ್ಮ ಕೋಡ್ ಸೇರಿಸಿ custom ಬ್ಲಾಕ್ ಆದ್ದರಿಂದ ಪ್ರಸ್ತುತ ಮೌಲ್ಯವನ್ನು ಬ್ಲಾಕ್ ಪರಿಶೀಲಿಸುತ್ತದೆ `score`{:class="block3variables"} ಮೌಲ್ಯಕ್ಕಿಂತ ದೊಡ್ಡದಾಗಿದೆ `high score`{:class="block3variables"} ವೇರಿಯಬಲ್, ತದನಂತರ ಮೌಲ್ಯವನ್ನು ಸಂಗ್ರಹಿಸುತ್ತದೆ `score`{:class="block3variables"} ಹೊಸ ಮೌಲ್ಯದಂತೆ `high score`{:class="block3variables"}.

![ಹಂತ sprite](images/stage-sprite.png)

```blocks3
    define check high score
    if <(score :: variables) > (high score)> then
        set [high score v] to (score :: variables)
    end
```

--- /task ---

--- task ---

ಸ್ಕ್ರಿಪ್ಟ್ ಮುಗಿಯುವ ಮೊದಲು ನಿಮ್ಮ ಹೊಸ custom ಬ್ಲಾಕ್ಅನ್ನು ಸ್ಟೇಜ್ ಸ್ಕ್ರಿಪ್ಟ್‌ಗೆ ಸೇರಿಸಿ.

![ಹಂತ sprite](images/stage-sprite.png)

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

ನಿಮ್ಮ score ಸರಿಯಾಗಿ ಉಳಿತಾಯವಾಗಿದೆಯೇ ಎಂದು ಪರಿಶೀಲಿಸಲು ನಿಮ್ಮ ಆಟವನ್ನು 2 ಬಾರಿ ಆಟವಾಡಿ `high score`{:class="block3variables"}.

--- /task ---