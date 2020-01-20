## 더 많은 점 만들기

\--- task \---

Duplicate your 'red' dot sprite twice, and name the two new sprites 'yellow' and 'blue'.

![screenshot](images/dots-more-dots.png)

\--- /task \---

\--- task \---

Change the costume of each new sprite so it is the correct colour: the 'yellow' sprite should be yellow, and the 'blue' sprite should be blue.

\--- /task \---

\--- task \---

Change the code of each sprite so that the player has to match dot clone to the correct colour on the controller to score points.

![screenshot](images/dots-all-test.png)

\--- hints \---

\--- hint \---

This is the code you need to find and alter for both new sprites:

![screenshot](images/dots-more-dots.png)

```blocks3
    만약 <touching color [#FF0000]?> \(이\) 라면 
  [score v] 을\(를\) (1) 만큼 바꾸기
  (pop v) 재생하기
  . . .
    끝
```

\--- /hint \---

\--- hint \---

This is how you need to change the code for the yellow sprite:

```blocks3
    만약 <[#FFFF00] 색에 닿았는가?  :: +> \(이\)라면 
  [score v] 을\(를\) (1) 만큼 바꾸기
  (pop v) 재생하기
end
```

This is how you need to change the code for the blue sprite:

```blocks3
    만약 <[#0000FF] 색에 닿았는가? :: +> \(이\)라면 
  [score v] 을\(를\) (1) 만큼 바꾸기
  (pop v) 재생하기
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---

If you play the game now, you can see that the dots sometimes get created one top of each other.

\--- task \---

Change the code for the 'yellow' dot sprite so that it waits four seconds after the flag is clicked before appearing.

![Yellow dot](images/yellow-sprite.png)

```blocks3
    ⚑ 클릭했을 때
숨기기
+ (4) 초 기다리기
```

![Blue dot](images/blue-sprite.png)

Then change the code for the 'blue' dot sprite so that it waits 6 seconds after the flag is clicked before appearing.

\--- /task \---