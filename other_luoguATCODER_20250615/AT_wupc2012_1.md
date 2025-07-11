# AT_wupc2012_1 招待状

## 题目描述

[problemUrl]: https://atcoder.jp/contests/wupc2012/tasks/wupc2012_1

 「WUPCへようこそ」  
  
 ある日，僕のもとに一通のメールが届いた．誰からは不明だが，プログラミングコンテストへの招待状であることはすぐに分かった．2012年現在，プログラミングコンテストは学生有志によって頻繁に開催されており，そのようなコンテストには日本中から競技プログラマが集まってくる．腕試しのため，僕も参加することにしよう．  
  
 とりあえず肩慣らしとして，現在の日付と開催予定日から，今日から数えて開催日まであと何日あるかを求めるプログラムを作ってみよう． メールを受け取った日付と，コンテスト開催日の日付が標準入力から与えられる．両者はどちらも2012年の日付である．メールを受け取った日付から数えて，コンテスト開催日まであと何日あるかを標準出力に出力するプログラムを作成せよ． 入力は以下の形式で標準入力から与えられる．

> $ M_{a}　D_{a} $ $ M_{b}　D_{b} $

- 1行目はメールを受け取った日付の月 $ M_{a} $($ 1\ ≦\ M_{a}\ ≦\ 12 $) と日 $ D_{a} $($ 1\ ≦\ D_{a}\ ≦\ 31 $)が半角スペース区切りで与えられる．
- 2行目はコンテスト開催日の月 $ M_{b} $($ 1\ ≦\ M_{b}\ ≦\ 12 $) と日 $ D_{b} $($ 1\ ≦\ D_{b}\ ≦\ 31 $)が半角スペース区切りで与えられる．
- $ M_{b} $ 月 $ D_{b} $ 日が$ M_{a} $ 月 $ D_{a} $ 日と同じか，それより前の日付になることはない．
- $ 13 $ 月 $ 10 $ 日や $ 2 $ 月 $ 30 $ 日などの無効な日付が与えられることはない．
 
 メールを受け取った日付から数えて，コンテスト開催日まであと何日あるかを標準出力に $ 1 $ 行で出力せよ．  
 なお，最後には改行を出力せよ． $ 2012 $ 年における $ 1 $ 月〜 $ 12 $ 月までの最大日数は $ 1 $ 月から順番に， ```

31, 29, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31
```

 である． ```
<pre class="prettyprint linenums">
3 1
3 10
```

 ```
<pre class="prettyprint linenums">
9
```

 ```
<pre class="prettyprint linenums">
2 10
3 10
```

 ```
<pre class="prettyprint linenums">
29
```

- $ 2012 $ 年はうるう年のため，$ 2 $ 月は $ 29 $ 日ある．
- $ 2 $ 月が終わるまで $ 20 $ 日，$ 3/10 $ までは $ 3/1 $ から $ 9 $日あるため，それらの合計である $ 29 $ を出力する．

## 输入格式

无

## 输出格式

无