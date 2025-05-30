## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc131/tasks/abc131_f

$ 2 $ 次元平面上の $ N $ 個の点があり、$ i $ 番目の点の座標は $ (x_i,\ y_i) $ です。

以下の操作を行える限り繰り返します。

- 座標 $ (a,\ b),\ (a,\ d),\ (c,\ b),\ (c,\ d) $ のうちちょうど $ 3 $ 箇所に点が存在するような整数 $ a,\ b,\ c,\ d\ (a\ \neq\ c,\ b\ \neq\ d) $ を選び、残りの $ 1 $ 箇所に点を追加する。

この操作は有限回しか行なうことができないことが証明できます。操作回数の最大値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ x_1 $ $ y_1 $ $ : $ $ x_N $ $ y_N $

## 输出格式
操作回数の最大値を出力せよ。

## 题目大意
给定平面中的 $N$（$1 \le N \le {10}^5$）个点 $(x_i, y_i)$，（$1 \le x_i, y_i \le {10}^5$），你可以不断执行以下操作：

如果 $(ax,ay), (bx,ay), (ax,by)$ 均存在，且 $a \ne b$，$(bx, by)$ 不存在，就可以加入一个点 $(bx, by)$。

求最多可以执行多少次这样的操作。

```input1
3
1 1
5 1
5 5
```

```output1
1
```

```input2
2
10 10
20 20
```

```output2
0
```

```input3
9
1 1
2 1
3 1
4 1
5 1
1 2
1 3
1 4
1 5
```

```output3
16
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ x_i,\ y_i\ \leq\ 10^5 $
- $ x_i\ \neq\ x_j $ または $ y_i\ \neq\ y_j\ (i\ \neq\ j) $
- 入力は全て整数である

### Sample Explanation 1

$ a\ =\ 1,\ b\ =\ 1,\ c\ =\ 5,\ d\ =\ 5 $ とすると $ (1,\ 5) $ に点を追加することができます。これ以上操作を行うことはできないので、操作回数の最大値は $ 1 $ 回です。

### Sample Explanation 2

$ 2 $ 点しか点がないので操作を $ 1 $ 回も行うことができません。

### Sample Explanation 3

$ a\ =\ 1,\ b\ =\ 1,\ c\ =\ i,\ d\ =\ j\ (2\ \leq\ i,j\ \leq\ 5) $ の全てに対して操作を行うことができ、それ以上操作を行うことはできないので、操作回数の最大値は $ 16 $ 回です。

