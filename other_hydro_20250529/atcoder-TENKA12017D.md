## 题目描述
[problemUrl]: https://atcoder.jp/contests/tenka1-2017/tasks/tenka1_2017_d

非負整数専門店「せいすうや」には、$ N $ 個の非負整数が売られています。$ i $ 個目の非負整数は $ A_i $ で、その価値は $ B_i $ です。 価値の異なる同じ非負整数が複数売られていることもあります。

高橋君は、「せいすうや」でいくつかの整数を買うことにしました。高橋君は、買う整数たちの bitwise or が $ K $ 以下になるような 任意の組み合わせで、整数を買うことができます。高橋君は、買った整数たちの価値の総和をできるだけ大きくしたいです。

高橋君が達成できる、価値の総和の最大値を求めてください。ただし、bitwise or とは、ビットごとの論理和を表します。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ A_1 $ $ B_1 $ : $ A_N $ $ B_N $

## 输出格式
高橋君が達成できる価値の総和の最大値を出力せよ。

## 题目大意
给定$N$ $(1\leq N\leq 10^5)$个数，每个数有一个$A$值$(0\leq A_i<2^{30}(1\leq i\leq N))$和一个$B$值$(1\leq B_i\leq 10^9(1\leq i\leq N))$，从中选取若干个数，使得在$A$值按位或(OR)不大于$K$ $(0\leq K<2^{30})$的约束下，$B$值之和最大

**保证所有数为正整数**

输入：

$N\ K$

$A_1\ B_1$

$\dots $

$A_N\ B_N$

输出：最大的$B$值之和

```input1
3 5
3 3
4 4
2 5
```

```output1
8
```

```input2
3 6
3 3
4 4
2 5
```

```output2
9
```

```input3
7 14
10 5
7 4
11 4
9 8
3 6
6 2
8 9
```

```output3
32
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ 0\ \leq\ K\ <\ 2^{30} $
- $ 0\ \leq\ A_i\ <\ 2^{30}(1\leq\ i\leq\ N) $
- $ 1\ \leq\ B_i\ \leq\ 10^9(1\leq\ i\leq\ N) $
- 入力は全て整数である

### Sample Explanation 1

$ 2 $ と $ 3 $ を購入することで、最大値 $ 8 $ を達成できます。

### Sample Explanation 2

$ 2 $ と $ 4 $ を購入することで、最大値 $ 9 $ を達成できます。

