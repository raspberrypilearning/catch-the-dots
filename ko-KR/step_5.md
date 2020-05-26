## 난이도 올리기

이제 당신은 게임이 진행될수록 게임이 더 어려워지게 만들겁니다. 점들이 점점 더 빠르게 나타나게 하면 게임이 어려워질 것입니다.

--- task ---

새 `변수`{:class="block3variables"}를 만들고 '지연 시간'이라는 이름을 붙이세요

![무대 스프라이트](images/stage-sprite.png)

--- /task ---

--- task ---

스테이지의 스크립트 부분으로 가서 새 스크립트를 생성하고 변수 `지연 시간`{:class="block3variables"}을 `8`로 설정하고 게임이 진행될수록 `지연 시간`{:class="block3variables"}의 값이 줄어들게 하세요.

![무대 스프라이트](images/stage-sprite.png)

```blocks3
  when flag clicked
	set [지연 시간 v] to (8)
	repeat until < (지연 시간) = (2)>
		wait (10) seconds
		change [지연 시간 v] by (-0.5)
	end
```

--- /task ---

이 코드는 타이머를 만들 때의 코드와 아주 비슷하다는 점을 알아두세요!

다음으로 빨강, 노랑, 파랑 스프라이트의 코드 스크립트에서 변수 `지연 시간`{:class="block3variables"}을 사용하세요.

--- task ---

임의의 시간 간격을 가지고 점 스프라이트가 복제되도록 만드는 코드 블럭을 삭제하세요. 당신이 지운 블럭을 변수 `지연 시간`{:class="block3variables"} 으로 바꾸세요.

![스크린샷](images/all-dots.png)

```blocks3
- 	wait (pick random (5) to (10)) secs
	  wait (지연 시간 :: variables) secs
```

세 점 스프라이트에 이 작업을 하세요.

--- /task ---

--- task ---

게임을 테스트하고, 게임이 진행될 수록 점들이 더 빨리 등장하는지 확인하세요.

+ 세가지 색의 점들 모두에서 제대로 작동하나요?
+ 변수 `지연 시간`{:class="block3variables"} 값이 줄어드는게 보이나요?

--- /task ---