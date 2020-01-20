## 조종기를 만들어 보세요

플레이어가 점을 잡을 때 이용할 조종기를 만들는 것부터 시작해 봅시다.

\--- task \---

Open the 'Catch the dots' Scratch starter project.

**Online:** open the starter project at [rpf.io/dots-on](http://rpf.io/dots-on){:target="_blank"}.

If you have a Scratch account you can make a copy by clicking **Remix**.

**Offline:** download the starter project from [rpf.io/p/en/catch-the-dots-go](http://rpf.io/p/en/catch-the-dots-go), and then open it in the Scratch offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](http://rpf.io/scratchoff).

\--- /task \---

You should see a controller sprite:

![screenshot](images/dots-controller.png)

\--- task \---

Add some code to the controller sprite to make the sprite turn right if the player presses the right arrow key:

![Controller sprite](images/controller-sprite.png)

```blocks3
    ⚑ 클릭했을 때
무한 반복하기 
  만약 <key (right arrow v) pressed?> \(이\)라면 
    ↻ 방향으로 (3) 도 회전하기
  end
end
```

\--- /task \---

\--- task \---

Test your code. The controller should spin to the right when you press the right arrow key.

\--- /task \---

\--- task \---

Add code to the controller sprite to make the sprite turn left if the player presses the left arrow key.

![Controller sprite](images/controller-sprite.png)

\--- hints \---

\--- hint \---

Find the code that checks whether the right arrow key is pressed and makes the sprite turn right. Can you add a copy of this code, and change the copy so it checks whether the left arrow key is pressed and makes the sprite turn left?

\--- /hint \---

\--- hint \---

Here are the blocks you need:

```blocks3
<(space v) 키를 눌렸는가?>

↺ 방향으로 (15) 도 회전하기
만약 <> \(이\)라면
end
```

\--- /hint \---

\--- hint \---

Here is what your code should look like:

```blocks3
    ⚑ 클릭했을 때
무한 반복하기 
  만약 <(right arrow v) 키를 눌렸는가?> \(이\)라면 
    ↻ 방향으로 (3) 도 회전하기
  end
  + 만약 <(left arrow v) 키를 눌렸는가?> \(이\)라면 
  +   ↺ 방향으로 (3) 도 회전하기
  + end
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---