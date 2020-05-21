## 최고 점수

당신은 게임의 최고 점수을 저장하여, 다른 플레이어에게 당신이 얼마나 잘 했는지 볼 수 있게 할 것입니다.

\--- task \---

먼저, `점수`{:class="block3variables"}라는 이름의 새 변수를 추가 해 보세요.

![무대 스프라이트](images/stage-sprite.png)

\--- /task \---

\--- task \---

스테이지 설정. '나만의 블록'을 클릭해서 `최고 점수 확인`{:class="block3myblocks"}라는 새로운 커스텀 블록을 만드세요.

![무대 스프라이트](images/stage-sprite.png)

![스크린샷](images/dots-custom-1.png)

\--- /task \---

\--- task \---

당신의 커스텀 블럭에 코드를 입력해서 현재 `점수`{:class="block3variables"}가 `최고 점수`{:class="block3variables"}보다 높은지 블럭이 확인해서 `최고 점수`{:class="block3variables"}를 현재의 `점수`{:class="block3variables"}로 바꾸게 하세요.

![무대 스프라이트](images/stage-sprite.png)

```blocks3
    최고 점수 정의하기
   만약 <(점수)>(최고 점수)> 이라면
      [최고 점수] 를 (점수) 로 바꾸기
   끝
```

\--- /task \---

\--- task \---

스크립트 마지막의 스테이지 스크립트에 새로운 커스텀 블럭을 추가하세요.

![무대 스프라이트](images/stage-sprite.png)

```blocks3
⚑ 클릭했을 때
[lives v] 을\(를\) (3) 로 정하기
[score v] 을\(를\) (0) 로 정하기
<(lives) < (1)> 까지 기다리기

+ 최고 점수를 확인하려면 
stop [all v]
```

\--- /task \---

\--- task \---

게임을 두 번 플레이 해서 당신의 점수가 `최고 점수`{:class="block3variables"}로 정확히 기록되는지 확인하세요.

\--- /task \---