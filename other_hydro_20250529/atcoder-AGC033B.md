## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc033/tasks/agc033_b

縦 $ H $ 行、横 $ W $ 列の長方形上のマス目があります。上から $ i $ 行目、左から $ j $ 列目のマスを $ (i,j) $ と表します。 このマス目の上には一つの駒が置いてあり、最初はマス $ (s_r,s_c) $ に置いてあります。

高橋君と青木君はそれぞれ長さ $ N $ の文字列を用意してゲームをすることにしました。 高橋君は文字列 $ S $ を、青木君は文字列 $ T $ を用意し、$ S $ と $ T $ はともに `L`, `R`, `U`, `D` の $ 4 $ 種類の文字からなります。

ゲームは $ N $ 回のステップからなります。$ i $ 回目のステップは以下のように進行します。

- まず高橋君が操作を行う。この操作では、駒を $ S_i $ の方向に動かす、もしくは、駒を動かさないかのいずれかを行う。
- 次に青木君が操作を行う。この操作では、駒を $ T_i $ の方向に動かす、もしくは、駒を動かさないかのいずれかを行う。

ここで、駒を `L`, `R`, `U`, `D` の方向に動かすとは、駒がマス $ (r,c) $ にあったとき、 それぞれマス $ (r,c-1) $, $ (r,c+1) $, $ (r-1,c) $, $ (r+1,c) $ に動かす操作を指します。 ただし、その座標に対応するマスが存在しない場合は、駒をマス目から取り除く操作を指すことにします。 この操作が行われた場合、$ N $ 回のステップが終わっていなくても、その時点でゲームは終了します。

高橋君は $ N $ 回のステップのいずれかのステップで駒をマス目から取り除きたいです。 一方で、青木君は最終的に駒がマス目上に残ったまま、$ N $ 回のステップを終えたいです。 二人が最適に行動したとき、ゲームが終了した時点で駒がマス目上に残っているかどうかを判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ N $ $ s_r $ $ s_c $ $ S $ $ T $

## 输出格式
ゲームが終了した時点で駒がマス目上に残っているならば `YES` を、 そうでないならば `NO` と出力せよ。

## 题目大意
有一个 $H$ 行 $W$ 列的棋盘，在 $(s_r,s_c)$ 处有一个棋子。

两人轮流进行 $n$ 步操作，在第 $i$ 步，先手可以按照 $S_i$ 移动棋子或者不动；后手可以按照 $T_i$ 移动棋子或者不动。

其中 $S_i,T_i\in\{U,D,L,R\}$ 分别表示向上，下，左，右移动一格。

**先手** 希望棋子某时刻走出棋盘，**后手** 希望棋子始终在棋盘上。

若两人均按照最优策略走，棋子能否 **始终在棋盘上** ？

```input1
2 3 3
2 2
RRL
LUD
```

```output1
YES
```

```input2
4 3 5
2 2
UDRRR
LLDUD
```

```output2
NO
```

```input3
5 6 11
2 1
RLDRRUDDLRL
URRDRLLDLRD
```

```output3
NO
```

## 提示
### 制約

- $ 2\ ≦\ H,W\ ≦\ 2\ \times\ 10^5 $
- $ 2\ ≦\ N\ ≦\ 2\ \times\ 10^5 $
- $ 1\ ≦\ s_r\ ≦\ H $
- $ 1\ ≦\ s_c\ ≦\ W $
- $ |S|=|T|=N $
- $ S $ と $ T $ は `L`, `R`, `U`, `D` の $ 4 $ 種類の文字からなる。

### Sample Explanation 1

ゲームは例えば以下のように進行します。 - 高橋君が駒を右に動かし、駒は $ (2,3) $ に移動する。 - 青木君が駒を左に動かし、駒は $ (2,2) $ に移動する。 - 高橋君は駒を動かさず、駒の位置は $ (2,2) $ のままとなる。 - 青木君は駒を上に動かし、駒は $ (1,2) $ に移動する。 - 高橋君は駒を左に動かし、駒は $ (1,1) $ に移動する。 - 青木君は駒を動かさず、駒の位置は $ (1,1) $ のままとなる。

