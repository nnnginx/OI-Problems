## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc198/tasks/abc198_f

立方体の各面に $ 1 $ つずつ正の整数を書きます。書かれた $ 6 $ つの数の和が $ S $ になるような書き込み方は何通りありますか？

ただし、立方体を回転した時に一致するような書き込み方は区別しないものとします(数に向きはありません)。

答えは非常に大きくなる可能性があるので、$ 998244353 $ で割ったあまりを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
答えを $ 998244353 $ で割った余りを出力せよ。

## 题目大意
### 题目描述

在立方体的六面各写下一个正整数，使得这些数的和为$S$。

如果两个立方体能够通过旋转使得对应面的数字都相同（数字不考虑朝向），则这两个立方体视为本质相同。

给定$S$，请问有多少个本质不同的立方体？答案对$998244353$取模。

### 输入数据

一个正整数$S,6\leqslant S\leqslant 10^{18}。$

### 输出数据

本质不同的立方体数量，答案对$998244353$取模。

### Sample Explanation 1

有两种数字的选择：

1. $1,1,1,1,1,3$，产生$1$个本质不同立方体
2. $1,1,1,1,2,2$，产生$2$个本质不同立方体（分别为两个$2$相邻或相对）

所以总共有$3$个本质不同立方体，答案为$3$。

### Sample Explanation 4

请将答案对$998244353$取模。

```input1
8
```

```output1
3
```

```input2
9
```

```output2
5
```

```input3
50
```

```output3
80132
```

```input4
10000000000
```

```output4
2239716
```

## 提示
### 制約

- $ 6\ \leq\ S\ \leq\ 10^{18} $
- $ S $ は整数

### Sample Explanation 1

書かれた $ 6 $ つの数が $ (1,1,1,1,1,3) $ であるような書き込み方が $ 1 $ 通り、$ (1,1,1,1,2,2) $ であるような書き込み方が $ 2 $ 通り ($ 2 $ が書かれた面が隣り合うものと反対側に配置されるもの) の、計 $ 3 $ 通りの書き込み方があります。

### Sample Explanation 4

答えを $ 998244353 $ で割ったあまりを求めてください。

