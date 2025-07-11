# AT_agc072_a [AGC072A] Rhythm Game

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc072/tasks/agc072_a

音楽に合わせて数直線上を走り回る、次のようなゲームを考えます。

> 数直線上に $ N $ 個のボタンがあります。$ i $ 番目 $ (1\ \leq\ i\ \leq\ N) $ のボタンは、ゲーム開始 $ T_i $ 秒後に座標 $ X_i $ に出現します。 また、どのボタンについても出現から $ D+0.5 $ 秒後に消えます。
> 
> プレイヤーは、ゲーム開始時に座標 $ 0 $ を出発し、$ N $ 個すべてのボタンを押すことができればゲームクリアとなります。ボタンは好きな順番で押して構いません。 しかし、本ゲームには特殊ルールがあり、ボタンを押してから次にボタンを押すまでの間に、毎回一度以上座標 $ 0 $ に移動する必要があります。それが守られない場合は失格となります。

AtCoder さんは、数直線上を秒速 $ 1 $ で移動することができます。彼女がゲームクリアする方法は存在しますか。 ただし、ボタンを押すのにかかる時間は無視できるものとします。

$ \mathrm{TESTCASES} $ 個のテストケースについて解いてください。

## 输入格式

入力は以下の形式で標準入力から与えられます。ここで、$ \mathrm{case}_k $ は $ k $ 番目のテストケースを意味します。

> $ \mathrm{TESTCASES} $ $ \mathrm{case}_1 $ $ \mathrm{case}_2 $ $ \vdots $ $ \mathrm{case}_{\mathrm{TESTCASES}} $

各テストケースは、以下の形式で与えられます。

> $ N $ $ D $ $ T_1 $ $ X_1 $ $ T_2 $ $ X_2 $ $ \vdots $ $ T_N $ $ X_N $

## 输出格式

$ \mathrm{TESTCASES} $ 行出力してください。$ k $ 行目には、$ k $ 番目のテストケースについて、ゲームクリアする方法が存在するならば `Yes`、存在しないならば `No` と出力してください。

## 输入输出样例 #1

### 输入 #1

```
4
2
10
30 20
50 10
2
9
30 20
50 10
4
185
0 40
0 30
0 20
0 10
5
1312372641
141421356 314159265
237309504 358979323
880168872 846264338
4209698078 327950288
5696718753 419716939
```

### 输出 #1

```
Yes
No
Yes
No
```

## 说明/提示

### 制約

- $ 1\ \leq\ \mathrm{TESTCASES}\ \leq\ 100\,000 $
- $ 1\ \leq\ N\ \leq\ 5\,000 $
- $ 0\ \leq\ D\ \leq\ 10^{12} $
- $ 0\ \leq\ T_1\ \leq\ T_2\ \leq\ \dots\ \leq\ T_N\ \leq\ 10^{12} $
- $ 1\ \leq\ X_i\ \leq\ 10^{12} $
- すべてのテストケースに対する $ N $ の総和は $ 100\,000 $ 以下である
- すべてのテストケースに対する $ N^2 $ の総和は $ 2.5\ \times\ 10^7 $ 以下である
- 入力される値はすべて整数

### Sample Explanation 1

1 番目のテストケースでは、以下のように動くとゲームクリアとなります。そのため、1 行目に `Yes` と出力します。 開始からの時間動作・出来事の説明$ 0 $ 秒ゲームが開始する。$ 5 $ 秒座標 $ 0 $ から右方向に移動を開始する。$ 25 $ 秒座標 $ 20 $ に到着し、停止する。$ 30 $ 秒$ 1 $ 番目のボタンが座標 $ 20 $ に出現する。ただちにこのボタンを押し、左方向に移動を開始する。$ 50 $ 秒座標 $ 0 $ に到着する。移動方向を右方向に変える。ちょうどそのタイミングで、$ 2 $ 番目のボタンが座標 $ 10 $ に出現する。$ 60 $ 秒座標 $ 10 $ に到着し、$ 2 $ 番目のボタンを押す。このボタンは開始 $ 60.5 $ 秒後に消えるので、間に合っている。2 番目のテストケースについては、ゲームクリアする方法が存在しないので、2 行目に `No` と出力します。 3 番目のテストケースについては、ゲームクリアする方法が存在するので、3 行目に `Yes` と出力します。 4 番目のテストケースについては、ゲームクリアする方法が存在しないので、4 行目に `No` と出力します。