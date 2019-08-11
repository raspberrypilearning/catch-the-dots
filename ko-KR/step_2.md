## 조종기를 만들어 보세요

플레이어가 점을 잡을 때 이용할 조종기를 만들는 것부터 시작해 봅시다.

\--- 할 일 \--- ‘점을 잡아라Catch the dots’ 파이썬(스크래치) 스타터 프로젝트를 엽니다.

**온라인 : ** [rpf.io/dots-on](http://rpf.io/dots-on){:target="_blank"}에서 스타터 프로젝트 열기.

스크래치 계정이 있는 경우 **Remix**을 클릭하여 사본을 만들 수 있습니다.

**오프라인 : ** [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go)에서 오프라인 시작 프로그램을 다운로드하고, 오프라인 에디터로 파일을 엽니다.

스크래치 오프라인 에디터를 설치해야 할 경우[rpf.io/scratchoff](http://rpf.io/scratchoff)에서 다운받을 수 있습니다.

\--- /task \---

스프라이트 컨트롤러(조종기)가 보일 것입니다 :

![screenshot](images/dots-controller.png)

스프라이트 컨트롤러(조종기)에 코드를 추가하여 오른쪽 방향키를 누르면 스프라이트가 오른쪽으로 회전하도록 만들어 보세요 :

![Controller sprite](images/controller-sprite.png)

```blocks3
    플래그를 클릭하면
    forever
        if <key (right arrow v) pressed?> then
            turn right (3) ˚(degrees. 도)
        end
    end
```

\--- /task \---

\--- task \--- 코드를 테스트 해 보세요. The controller should spin to the right when you press the right arrow key. \--- /task \---

\--- task \--- Add code to the controller sprite to make the sprite turn left if the player presses the left arrow key.

![Controller sprite](images/controller-sprite.png)

\--- hints \--- \--- hint \---

Find the code that checks whether the right arrow key is pressed and makes the sprite turn right. Can you add a copy of this code, and change the copy so it checks whether the left arrow key is pressed and makes the sprite turn left?

\--- /hint \--- \--- hint \--- Here are the blocks you need:

```blocks3
<key (space v) pressed?>

turn left(15) degrees

if <> then

end
```

\--- /hint \--- \--- hint \--- Here is what your code should look like:

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

\--- /hint \--- \--- /hints \--- \--- /task \---