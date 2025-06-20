# AT_arc109_d [ARC109D] く

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc109/tasks/arc109_d

<!-- $ 2\time\ 10^{10}\ +\ 1 $ 行 $ 2\time\ 10^{10}\ +\ 1 $ 列からなるマス目上に区切られた盤面があります。行には上から順番に $ -10^{10},\ \dots,\ 10^{10} $ の番号が、列には左から$ 2\time\ 10^{10}\ +\ 1 $ の場脳が振られています。この盤面の上に石が $ 3 $ つ置かれています。
 -->二次元平面上の点 $ (0,\ 0),\ (1,0),\ (0,1) $ に石がひとつずつ置かれています。

$ 3 $ つの石が次の条件を満たしているとき、くの字に並んでいるといいます。

- どの石も、座標が整数である点に置かれている
- どの石も、別の石と隣接している（石からの距離が $ 1 $ である場所に別の石が存在する）
- $ 3 $ つの石が一直線上に存在しない

特に、最初の石の並べ方 $ (0,\ 0),\ (1,0),\ (0,1) $ は、くの字です。

好きな石を $ 1 $ つ選んで好きな位置に移動させる操作を好きなだけできます。ただし、各操作後の石は、くの字に並んでいなければなりません。 できるだけ少ない操作回数で、石が点 $ (ax,\ ay),\ (bx,\ by),\ (cx,\ cy) $ にひとつずつ置かれている状態にしたいです。必要な操作回数は何回ですか？ただし、この状態で石がくの字に並んでいることは保証されます。この制約のもと、有限回の操作で目標を達成できます。

$ T $ 個のケースが与えられるので、それぞれについて答えを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ T $ $ \text{case}_1 $ $ \vdots $ $ \text{case}_T $

各ケースは以下の形式で与えられる。

> $ ax $ $ ay $ $ bx $ $ by $ $ cx $ $ cy $

## 输出格式

$ T $ 個の値を出力せよ。$ i $ 個目には $ \text{case}_i $ に対応する操作回数の最小値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
1
3 2 2 2 2 1
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
10
0 0 1 0 0 1
1 0 0 1 1 1
2 -1 1 -1 1 0
1 -2 2 -1 1 -1
-1 2 0 2 -1 3
-1 -2 -2 -2 -2 -3
-2 4 -3 3 -2 3
3 1 4 2 4 1
-4 2 -4 3 -3 3
5 4 5 3 4 4
```

### 输出 #2

```
0
1
2
3
4
5
6
7
8
9
```

## 说明/提示

### 注意

$ 3 $ つの石は互いに区別できないとします。例えば、最初に点 $ (0,0) $ に置かれていた石が最終的に点 $ (ax,\ ay),\ (bx,\ by),\ (cx,\ cy) $ のどこに置かれていても構いません。

### 制約

- $ 1\ \leq\ T\ \leq\ 10^3 $
- $ |ax|,|ay|,|bx|,|by|,|cx|,|cy|\ \leq\ 10^9 $
- 点 $ (ax,\ ay),\ (bx,\ by),\ (cx,\ cy) $ に石がひとつずつ置かれている時、石はくの字に並んでいる

### Sample Explanation 1

Let us use `#` to represent a stone. You can move the stones to the specified positions with four operations, as follows:

```
....    ....    ....    ..#.    ..##
#... -> ##.. -> .##. -> .##. -> ..#.
##..    .#..    .#..    ....    ....
```