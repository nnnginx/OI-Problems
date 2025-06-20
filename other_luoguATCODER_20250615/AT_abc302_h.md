# AT_abc302_h [ABC302Ex] Ball Collector

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc302/tasks/abc302_h

$ N $ 頂点の木があります。$ i(1\ \le\ i\ \le\ N-1) $ 本目の辺は、頂点 $ U_i $ と $ V_i $ を結ぶ無向辺です。頂点 $ i(1\ \le\ i\ \le\ N) $ には、$ A_i $ が書かれたボールと $ B_i $ が書かれたボールが $ 1 $ 個ずつあります。

$ v\ =\ 2,3,\dots,N $ に対して、以下の問題を解いてください。(各問題は独立です。)

- 頂点 $ 1 $ から頂点 $ v $ まで最短経路で移動します。このとき、通った各頂点(頂点 $ 1,v $ も含む)において、ボールを $ 1 $ 個ずつ選んで取ります。最終的に持っているボールに書かれている整数の種類数の最大値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ B_1 $ $ A_2 $ $ B_2 $ $ \vdots $ $ A_N $ $ B_N $ $ U_1 $ $ V_1 $ $ U_2 $ $ V_2 $ $ \vdots $ $ U_{N-1} $ $ V_{N-1} $

## 输出格式

$ v=2,3,\dots,N $ に対して、答えを空白区切りで出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4
1 2
2 3
3 1
1 2
1 2
2 3
3 4
```

### 输出 #1

```
2 3 3
```

## 输入输出样例 #2

### 输入 #2

```
10
2 5
2 2
8 8
4 3
6 10
8 1
9 10
1 7
9 3
5 10
9 3
1 9
3 6
4 1
3 8
10 9
5 4
7 2
9 7
```

### 输出 #2

```
4 3 2 3 4 3 4 2 3
```

## 说明/提示

### 制約

- $ 2\ \le\ N\ \le\ 2\ \times\ 10^5 $
- $ 1\ \le\ A_i,B_i\ \le\ N $
- 与えられるグラフは木である。
- 入力は全て整数である。
 
### Sample Explanation 1

例えば、$ v=4 $ のときは通る頂点は $ 1,2,3,4 $ であり、それぞれ $ A_1,B_2,B_3,B_4(=1,3,1,2) $ が書かれているボールを選ぶと種類数が $ 3 $ となり、これが最大となります。