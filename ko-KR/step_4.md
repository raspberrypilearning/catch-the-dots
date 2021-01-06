## 더 많은 점 만들기

\--- task \---

빨간 점 스프라이트를 두 번 복제하고 이름을 '노랑'과 '파랑'으로 설정하세요.

![스크린샷](images/dots-more-dots.png)

\--- /task \---

\--- task \---

각 스프라이트의 색을 알맞게 설정하세요. 예를 들면 노랑 스프라이트는 노란색이어야 하고, 파랑 스프라이트는 파란색이어야 합니다.

\--- /task \---

\--- task \---

각 스프라이트의 코드를 바꿔서 플레이어가 점수를 얻기 위해서 컨트롤러의 색과 점 복제본의 색을 맞추게 하세요.

![스크린샷](images/dots-all-test.png)

\--- hints \---

\--- hint \---

이것은 새로운 스프라이트에 들어가야 할 코드입니다.

![스크린샷](images/dots-more-dots.png)

```blocks3
    만약 <touching color [#FF0000]?> \(이\) 라면 
  [score v] 을\(를\) (1) 만큼 바꾸기
  (pop v) 재생하기
  . . .
    끝
```

\--- /hint \---

\--- hint \---

이것은 당신이 노랑 스프라이트에 넣어야 할 코드입니다:

```blocks3
    <[#FFFF00] 색에 닿았는가?  :: +> \(이\)라면 
  [score v] 을\(를\) (1) 만큼 바꾸기
  (pop v) 재생하기
end
```

이것은 당신이 파랑 스프라이트에 넣어야 할 코드입니다:

```blocks3
    <[#0000FF] 색에 닿았는가? :: +> \(이\)라면 
  [score v] 을\(를\) (1) 만큼 바꾸기
  (pop v) 재생하기
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---

If you play the game now, you can see that the dots sometimes get created on top of each other.

\--- task \---

'노랑' 점 스프라이트의 코드를 바꿔서 깃발이 클릭되고 4초 후에 나타나게 하세요.

![노랑 점](images/yellow-sprite.png)

```blocks3
    ⚑ 클릭했을 때
숨기기
+ (4) 초 기다리기
```

![파랑 점](images/blue-sprite.png)

그 다음, '파랑' 점 스프라이트의 코드를 바꿔서 깃발이 클릭되고 6초 후에 나타나게 하세요.

\--- /task \---