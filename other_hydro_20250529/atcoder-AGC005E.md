## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc005/tasks/agc005_e

しぐま君とすぎむ君はゲームをすることにしました。

このゲームは $ N $ 頂点のグラフの上で行います。頂点には $ 1,2,...,N $ と番号がついています。グラフには $ N-1 $ 本の赤い辺と $ N-1 $ 本の青い辺があり、どちらも木となっています。赤い辺は $ (a_i,\ b_i) $ で表し、青い辺は $ (c_i,\ d_i) $ で表します。

二人はそれぞれ駒を $ 1 $ 個ずつ持っており、しぐま君の駒の初期位置は頂点 $ X $、すぎむ君の駒の初期位置は頂点 $ Y $ です。

このゲームはターン制で、ターン $ 1 $, ターン $ 2 $, ターン $ 3 $, ... と進んでいきます。そして、ターン $ 1,\ 3,\ 5,\ ... $ はしぐま君、ターン $ 2,\ 4,\ 6,\ ... $ はすぎむ君の手番です。

二人は自分の手番では、自分の駒を動かすかパスをします。ただし動かせる頂点には制限があり、しぐま君は赤い辺、すぎむ君は青い辺で隣り合った頂点のみに駒を動かせます。

もし二つの駒が同じ頂点に来るとその時点でゲームは終了します。そしてターン $ i $ での操作の後にゲームが終了したならば、$ i $ を総ターン数とします。

しぐま君は総ターン数を出来る限り大きく、すぎむ君は出来る限り小さくしたいです。

二人はこの目的のもとで最適に行動をすると仮定したとき、ゲームは終了するかを判定し、終了する場合は総ターン数はいくつになるか求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ X $ $ Y $ $ a_1 $ $ b_1 $ $ a_2 $ $ b_2 $ : $ a_{N-1} $ $ b_{N-1} $ $ c_1 $ $ d_1 $ $ c_2 $ $ d_2 $ : $ c_{N-1} $ $ d_{N-1} $

## 输出格式
$ 1 $ 行に答えを出力する。 ただし、いつまでもゲームが終了しない場合は `-1` を出力する。

## 题目大意
现在 A 和 B 在玩游戏，游戏是在两棵树上进行的，A 在树 $a$ 上的点 $x$，B 在树 $b$ 上的点 $y$，两棵树上的点的编号是相同的，只是连边方式不同。

对于奇数轮，A 可以选择走到它当前在树 $a$ 上的点的相邻节点，或者在原地不动，对于偶数轮则是 B 进行选择，当两个人到达编号相同的点时，游戏结束。

现在 A 想最大化游戏轮数，B 想最小化游戏轮数。问游戏的轮数，如果可以进行无限轮游戏，请输出 $-1$。

```input1
4 1 2
1 2
1 3
1 4
2 1
2 3
1 4
```

```output1
4
```

```input2
3 3 1
1 2
2 3
1 2
2 3
```

```output2
4
```

```input3
4 1 2
1 2
3 4
2 4
1 2
3 4
1 3
```

```output3
2
```

```input4
4 2 1
1 2
3 4
2 4
1 2
3 4
1 3
```

```output4
-1
```

```input5
5 1 2
1 2
1 3
1 4
4 5
2 1
1 3
1 5
5 4
```

```output5
6
```

## 提示
### 制約

- $ 2\ ≦\ N\ ≦\ 200,000 $
- $ 1\ ≦\ X,\ Y\ ≦\ N $
- $ X\ \neq\ Y $
- $ 1\ ≦\ a_i,\ b_i,\ c_i,\ d_i\ ≦\ N $
- 赤い辺と青い辺はそれぞれ木である

### Sample Explanation 1

!\[\](https://atcoder.jp/img/agc005/0f55f48518cb9031ee9f1cc30f686228.png)

### Sample Explanation 2

!\[\](https://atcoder.jp/img/agc005/df982a9959ce46d5d5f63800f8972bff.png)

### Sample Explanation 3

!\[\](https://atcoder.jp/img/agc005/11ce9a2283a853025b7075769439d745.png)

