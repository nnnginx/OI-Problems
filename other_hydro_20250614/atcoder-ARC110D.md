## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc110/tasks/arc110_d

長さが $ N $ の非負整数列 $ A $ があります。

長さが $ N $ で、和が $ M $ 以下である任意の非負整数列 $ B $ について、$ \prod\ _{i\ =\ 1}\ ^N\ \dbinom{B_i}{A_i} $ の値を計算し、その総和を $ 10^9\ +\ 7 $ で割った余りを出力してください。

ここで $ \dbinom{B_i}{A_i} $ は、$ B_i $ 個のものの中から $ A_i $ 個のものを選ぶ場合の数（二項係数）であり、$ B_i\ <\ A_i $ のときは $ 0 $ です。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式
$ \prod\ _{i\ =\ 1}\ ^N\ \dbinom{B_i}{A_i} $ の総和を $ 10^9\ +\ 7 $ で割った余りを出力せよ。

## 题目大意
### 题目描述

我们有一个包含 $N$ 个非负整数的序列 $A$。

对于所有长度为 $N$ 且和不超过 $M$ 的非负整数序列 $B$，求 $\prod_{i = 1}^N {B_i \choose A_i}$ 之和， 对 $(10^9 + 7)$ 取模。

### 数据范围

- $1 \le N \le 2000$
- $1 \le M \le 10^9$
- $0 \le A_i \le 2000$



### 输入格式

第一行输入两个整 $N, M$，第二行 $N$ 个整数，表示序列 $A$。

### 输出格式

一行，表示答案对 $(10^9 + 7)$ 取模的值。





### 样例解释1

有四个序列 $B$ 满足 $\prod_{i=1}^N {B_i \choose A_i}$ 至少为 $1$：
	
- $B = \{1, 2, 1\}, \prod_{i = 1}^N{B_i \choose A_i} = {1 \choose 1} \times {2 \choose 2} \times {1 \choose 1} = 1$;
- $B = \{2, 2, 1\}, \prod_{i = 1}^N{B_i \choose A_i} = {2 \choose 1} \times {2 \choose 2} \times {1 \choose 1} = 2$;
- $B = \{1, 3, 1\}, \prod_{i = 1}^N{B_i \choose A_i} = {1 \choose 1} \times {3 \choose 2} \times {1 \choose 1} = 3$;
- $B = \{1, 2, 2\}, \prod_{i = 1}^N{B_i \choose A_i} = {1 \choose 1} \times {2 \choose 2} \times {2 \choose 1} = 2$.

它们的答案之和为 $1+2+3+2=8$。

###### $\text{\tiny{Translated by @nr0728.}}$

```input1
3 5
1 2 1
```

```output1
8
```

```input2
10 998244353
31 41 59 26 53 58 97 93 23 84
```

```output2
642612171
```

## 提示
### 制約

- 入力は全て整数
- $ 1\ \leq\ N\ \leq\ 2000 $
- $ 1\ \leq\ M\ \leq\ 10^9 $
- $ 0\ \leq\ A_i\ \leq\ 2000 $

### Sample Explanation 1

$ \prod\ _{i\ =\ 1}\ ^N\ \dbinom{B_i}{A_i} $ が $ 1 $ 以上となるような数列 $ B $ の定め方は、以下の $ 4 $ 通りです。 - $ B\ =\ 1,\ 2,\ 1 $ とする。このとき $ \prod\ _{i\ =\ 1}\ ^N\ \dbinom{B_i}{A_i}\ =\ \dbinom{1}{1}\ \times\ \dbinom{2}{2}\ \times\ \dbinom{1}{1}\ =\ 1 $ である - $ B\ =\ 2,\ 2,\ 1 $ とする。このとき $ \prod\ _{i\ =\ 1}\ ^N\ \dbinom{B_i}{A_i}\ =\ \dbinom{2}{1}\ \times\ \dbinom{2}{2}\ \times\ \dbinom{1}{1}\ =\ 2 $ である - $ B\ =\ 1,\ 3,\ 1 $ とする。このとき $ \prod\ _{i\ =\ 1}\ ^N\ \dbinom{B_i}{A_i}\ =\ \dbinom{1}{1}\ \times\ \dbinom{3}{2}\ \times\ \dbinom{1}{1}\ =\ 3 $ である - $ B\ =\ 1,\ 2,\ 2 $ とする。このとき $ \prod\ _{i\ =\ 1}\ ^N\ \dbinom{B_i}{A_i}\ =\ \dbinom{1}{1}\ \times\ \dbinom{2}{2}\ \times\ \dbinom{2}{1}\ =\ 2 $ である よって答えは $ 1\ +\ 2\ +\ 3\ +\ 2\ =\ 8 $ です。

