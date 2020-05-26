## 조종기를 만들어 보세요

플레이어가 점을 잡을 때 이용할 조종기를 만들는 것부터 시작해 봅시다.

--- task ---

'점을 잡아라' 파이썬(스크래치) 스타터 프로젝트를 엽니다.

**온라인:** [scratch.mit.edu/projects/399147808](https://scratch.mit.edu/projects/399147808){:target="_blank"}에서 스타터 프로젝트를 열 수 있습니다.

Scratch 계정이 있다면, **Remix**를 클릭하여 복사본을 만들 수 있습니다.

**인터넷이 없는경우:** [rpf.io/p/ko-KR/catch-the-dots-go](http://rpf.io/p/ko-KR/catch-the-dots-go)에서 스타터 프로젝트를 다운로드하고, Scratch 오프라인 에디터로 프로젝트를 열어주세요

만약 Scratch 오프라인 에디터가 없는경우 [rpf.io/scratchoff](http://rpf.io/scratchoff)를 통해서 다운받을 수 있습니다.

--- /task ---

스프라이트 컨트롤러(조종기)가 보일 것입니다 :

![스크린샷](images/dots-controller.png)

--- task ---

스프라이트 컨트롤러(조종기)에 코드를 추가하여 오른쪽 방향키를 누르면 스프라이트가 오른쪽으로 회전하도록 만들어 보세요:

![컨트롤러 스프라이트](images/controller-sprite.png)

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

코드를 테스트 해보세요. 오른쪽 방향키를 누르면 조종기는 시계방향으로 돌아야 합니다.

--- /task ---

--- task ---

코드를 추가해서 스프라이트 조종기를 왼쪽 방향키를 눌렀을 때 조정기가 왼쪽으로 돌아갈 수 있도록 만들어 보세요.

![컨트롤러 스프라이트](images/controller-sprite.png)

--- hints ---


--- hint ---

오른쪽 화살표를 누르면 스프라이트가 오른쪽으로 회전하도록 하는 코드를 찾아 보세요. 왼쪽 화살표 키를 누르면 스프라이트가 오른쪽으로 이동하는 코드를 응용할 수 있습니까?

--- /hint ---

--- hint ---

필요한 코드 블록은 다음과 같습니다.

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

--- /hint ---

--- hint ---

코드는 다음과 같이 설계되어야 합니다:

```blocks3
  when flag clicked
	forever
		if <key (right arrow v) pressed?> then
			turn right (3) degrees
		end
+ 		if <key (left arrow v) pressed?> then
			turn left(3) degrees
		end
	end
```

--- /hint ---

--- /hints ---

--- /task ---