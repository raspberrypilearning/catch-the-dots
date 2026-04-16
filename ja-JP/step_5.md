## 難易度を上げる

次に、プレイヤーがプレイする時間が長いほど、ゲームをより難しくします。 これを行うには、ドットが次第に速く表示されるようにします。

--- task ---

新しい「遅れ」`変数`{:class="block3variables"}を作成します。

![ステージのスプライト](images/stage-sprite.png)

--- /task ---

--- task ---

ステージのスクリプト領域に移動し、新しいスクリプトを作成します。`遅れ`{:class="block3variables"}変数を`8` に設定し、ゲームの実行中に`遅れ`{:class="block3variables"}の値をゆっくりと減らします。

![ステージのスプライト](images/stage-sprite.png)

```blocks3
	when flag clicked
	set [遅れ v] to (8)
	repeat until < (遅れ) = (2)>
		wait (10) seconds
		change [遅れ v] by (-0.5)
	end
```

--- /task ---

このコードは、カウントダウンタイマーの作成に使用するコードと非常に似ていることに注意してください。

次に、「赤」、「黄」、および「青」のスプライトのコードスクリプト内で `遅れ`{:class="block3variables"}変数を使用します。

--- task ---

ドットスプライトのクローンを作成する間にゲームをランダムな秒数だけ待機させるコードブロックを削除します。 そして削除したブロックを新しい`遅れ`{:class="block3variables"}変数に置き換えます。

![スクリーンショット](images/all-dots.png)

```blocks3
- 	wait (pick random (5) to (10)) secs
	wait (遅れ :: variables) secs
```

これを3つのドットスプライトすべてに対して行います。

--- /task ---

--- task ---

ゲームをテストし、ゲームが進むにつれてドットがより早く現れ始めるかどうかを確認します。

+ これは、3つの色付きドットすべてで機能しますか？
+ `遅れ`{:class="block3variables"}変数の値が減少するのがわかりますか？

--- /task ---