## ಅಂಕಗಳನ್ನು ಗಳಿಸಿ ಅಥವಾ ಪ್ರಾಣ ಕಳೆದುಕೊಳ್ಳಿ

ಈಗ ನೀವು ಆಟಗಾರನು ಸಂಗ್ರಹಿಸಬೇಕಾದ ಕೆಲವು ಚುಕ್ಕೆಗಳನ್ನು ಸೇರಿಸಲು ಹೊರಟಿದ್ದೀರಿ.

--- task ---

'red'(ಕೆಂಪು) ಎಂಬ ಹೊಸ sprite ರಚಿಸಿ. ಈ sprite ಸಣ್ಣ red ಚುಕ್ಕೆ ಆಗಿರಬೇಕು.

![Red ಚುಕ್ಕೆ sprite](images/dots-red.png)

--- /task ---

--- task ---

ಪ್ರತಿ ಕೆಲವು ಸೆಕೆಂಡುಗಳಲ್ಲಿ sprite‌ನ ಹೊಸ clone ರಚಿಸಲು ಈ ಸ್ಕ್ರಿಪ್ಟ್‌ ಅನ್ನು ನಿಮ್ಮ 'ಕೆಂಪು' sprite ಸೇರಿಸಿ:

![Red ಚುಕ್ಕೆ sprite](images/red-sprite.png)

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

ನೀವು ಈಗ green flag ಅನ್ನು ಕ್ಲಿಕ್ ಮಾಡಿದರೆ, ಏನೂ ಆಗುತ್ತಿಲ್ಲ ಎಂದು ತೋರುತ್ತಿದೆ. Cloned sprites ಗಳೆಲ್ಲವನ್ನು ಮರೆಮಾಡಲಾಗಿದೆ ಮತ್ತು ಅವು ಒಂದೇ ಸ್ಥಳದಲ್ಲಿ ಗೋಚರಿಸುತ್ತವೆ ಎಂಬುದು ಇದಕ್ಕೆ ಕಾರಣ.

ಪ್ರತಿ ಹೊಸ clone ಹಂತದ 4 ಮೂಲೆಗಳಲ್ಲಿ ಒಂದರಲ್ಲಿ ಗೋಚರಿಸುವಂತೆ ನೀವು ಕೋಡ್ ಅನ್ನು ಸೇರಿಸಲಿದ್ದೀರಿ.

![screenshot](images/dots-start.png)

--- task ---

ಹೊಸ ಪಟ್ಟಿಯನ್ನು ರಚಿಸಿ `start positions`{:class="block3variables"}, ಪಟ್ಟಿಯನ್ನು ಕ್ಲಿಕ್ ಮಾಡಿ `(+)` icon ಮೌಲ್ಯಗಳನ್ನು ಸೇರಿಸಲು `-180`{:class="block3variables"} ಮತ್ತು `180`{:class="block3variables"}.

![Red ಚುಕ್ಕೆ sprite](images/red-sprite.png)

![ಪಟ್ಟಿಗಳು 180 ಮತ್ತು -180](images/dots-list.png)

[[[generic-scratch3-make-list]]]

ಈ ಪೆಟ್ಟಿಗೆಯನ್ನು ಆಯ್ಕೆ ಮಾಡದಿರುವ ಮೂಲಕ ನೀವು ಪಟ್ಟಿಯನ್ನು ಮರೆಮಾಡಬಹುದು:

![ಪಟ್ಟಿಯನ್ನು ಮರೆಮಾಡಿ](images/hide-list.png)

--- /task ---

ಹಂತದ ಪ್ರತಿಯೊಂದು ಮೂಲೆಯ ನಿರ್ದೇಶಾಂಕವು ಒಂದು ಸಂಯೋಜನೆಯಾಗಿದೆ ಎಂಬುದನ್ನು ಗಮನಿಸಿ `180` ಮತ್ತು `-180`. ಇದರರ್ಥ ನೀವು ಹಂತದ ಒಂದು ಮೂಲೆಯನ್ನು ಆರಿಸಲು ಪಟ್ಟಿಯನ್ನು ಬಳಸಬಹುದು ಹಂತದ random.

--- task ---

ಈ ಕೋಡ್ ಅನ್ನು ಸೇರಿಸಿ 'dot' sprite ಗೆ ಪ್ರತಿಯೊಂದನ್ನು ಹೊಸದಾಗಿ sprite clone ಮಾಡಲು ಕಾಣಿಸಿಕೊಳ್ಳುತ್ತದೆ random corner ನಲ್ಲಿ ತದನಂತರ ನಿಧಾನವಾಗಿ ಕಂಟ್ರೊಲ್ರ್ sprite ಕಡೆಗೆ ಸರಿಸಿ.

![Red ಚುಕ್ಕೆ sprite](images/red-sprite.png)

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

ಈ ಹೊಸ ಕೋಡ್ ಆಯ್ಕೆ ಮಾಡುತ್ತದೆ `-180` ಅಥವಾ `180` ಗಾಗಿ x ಮತ್ತು y positions(ಸ್ಥಾನಗಳು), ಅಂದರೆ ಪ್ರತಿಯೊಂದೂ 'dot' sprite clone starts(ಪ್ರಾರಂಭವಾಗುತ್ತದೆ) ಹಂತದ ಒಂದು ಮೂಲೆಯಲ್ಲಿ.

--- task ---

ನಿಮ್ಮ ಯೋಜನೆಯನ್ನು ಪರೀಕ್ಷಿಸಿ. ಹಂತದ ಮೂಲೆಗಳಲ್ಲಿ red ಚುಕ್ಕೆಗಳು ಗೋಚರಿಸುವುದನ್ನು ನೀವು ನೋಡಬೇಕು ಮತ್ತು ಕಂಟ್ರೊಲ್ರ್ ಕಡೆಗೆ ನಿಧಾನವಾಗಿ ಚಲಿಸಬೇಕು.

![screenshot](images/dots-red-test.png)

--- /task ---

--- task ---

ಎರಡು ಹೊಸ variables ರಚಿಸಿ ಅವು `lives`{:class="block3variables"} ಮತ್ತು `score`{:class="block3variables"}.

![Red ಚುಕ್ಕೆsprite](images/red-sprite.png)

--- /task ---

--- task ---

ಆಟದ ಪ್ರಾರಂಭದಲ್ಲಿ ಹೊಂದಿಸಲು ನಿಮ್ಮ ಹಂತಕ್ಕೆ `lives`{:class="block3variables"} ಗೆ variable `3` ಮತ್ತು `score`{:class="block3variables"} ರಿಂದ `0` ಆಟದ ಪ್ರಾರಂಭದಲ್ಲಿ. ![ಹಂತ(stage) sprite](images/stage-sprite.png)

```blocks3
when flag clicked
set [lives v] to (3)
set [score v] to (0)
```

--- /task ---

--- task ---

ಆಟಗಾರನು ಜೀವನದ ಕೊನೆಯ ಭಾಗವನ್ನು ಕಳೆದುಕೊಂಡಾಗ ಆಟವನ್ನು ಕೊನೆಗೊಳಿಸಲು ಈ ಕೋಡ್ ಅನ್ನು ಹಂತದ ಸ್ಕ್ರಿಪ್ಟ್(script) ಕೊನೆಯಲ್ಲಿ ಸೇರಿಸಿ:

![ಹಂತ(Stage) sprite](images/stage-sprite.png)

```blocks3
    wait until <(lives :: variables) < [1]>
    stop [all v]
```

--- /task ---

ಆಟಗಾರನು ಚುಕ್ಕೆಗಳನ್ನು ಹಿಡಿಯಲು ಅಂಕಗಳನ್ನು ಗೆಲ್ಲಬೇಕು ಮತ್ತು ಚುಕ್ಕೆಗಳನ್ನು ಹಿಡಿಯಲು ವಿಫಲವಾದ ಕಾರಣ ಜೀವಗಳನ್ನು ಕಳೆದುಕೊಳ್ಳಬೇಕು. ಕಂಟ್ರೊಲ್ರ್ ಬಣ್ಣವನ್ನು ಚುಕ್ಕೆ ಬಣ್ಣಕ್ಕೆ ಹೊಂದಿಸುವುದರ ಮೂಲಕ ಮಾತ್ರ ಚುಕ್ಕೆ ಹಿಡಿಯಬಹುದು.

--- task ---

ಕೆಲವು ಕೋಡ್ ಬ್ಲಾಕ್‌ಗಳನ್ನು ಸೇರಿಸಲು 'red' ಡಾಟ್ ಸ್ಪ್ರೈಟ್‌ನ ಸ್ಕ್ರಿಪ್ಟ್‌ಗಳ ಪ್ರದೇಶಕ್ಕೆ ಹಿಂತಿರುಗಿ sprite's ಕೊನೆಯಲ್ಲಿ `when I start as a clone`{:class="block3control"} ಸ್ಕ್ರಿಪ್ಟ್.

ಮೊದಲಿಗೆ, dot clone ಮಾಡಿ `move 5 steps`{:class="block3motion"} ಆದ್ದರಿಂದ ಅದು ನಿಯಂತ್ರಕವನ್ನು ಅತಿಕ್ರಮಿಸುತ್ತದೆ.

ನಂತರ ಸೇರಿಸಲು ಕೋಡ್ ಸೇರಿಸಿ `1` ಗೆ `score`{:class="block3variables"} ಚುಕ್ಕೆಯ ಬಣ್ಣವಾಗಿದ್ದರೆ clone ಬಣ್ಣಕ್ಕೆ ಹೊಂದಿಕೆಯಾಗುತ್ತದೆ ಕಂಟ್ರೊಲ್ರ್ ಅವರು ಸ್ಪರ್ಶಿಸಿದಾಗ ಅಥವಾ ತೆಗೆದುಕೊಳ್ಳಲು `1` ನಿಂದ ದೂರ `lives`{:class="block3variables"} ಅವುಗಳ ಬಣ್ಣಗಳು ಹೊಂದಿಕೆಯಾಗದಿದ್ದರೆ.

[[[generic-scratch3-sound-from-library]]]

![Red ಚುಕ್ಕೆ sprite](images/red-sprite.png)

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

ಅದನ್ನು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಲು ನಿಮ್ಮ ಆಟವನ್ನು ಪರೀಕ್ಷಿಸಿ:

1. ನೀವು ಸರಿಯಾದ ಬಣ್ಣದೊಂದಿಗೆ ಚುಕ್ಕೆಗೆ ಹೊಂದಿಕೆಯಾಗದಿದ್ದರೆ ನೀವು ಜೀವನವನ್ನು ಕಳೆದುಕೊಳ್ಳುತ್ತೀರಿ
2. ನೀವು ಡಾಟ್ ಅನ್ನು ಸರಿಯಾಗಿ ಹೊಂದಿಸಿದರೆ ನೀವು ಪಾಯಿಂಟ್ ಗಳಿಸುತ್ತೀರಿ

--- /task ---