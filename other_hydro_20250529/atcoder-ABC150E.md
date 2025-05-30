## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc150/tasks/abc150_e

$ 0,\ 1 $ からなる長さ $ N $ の異なる $ 2 $ つの数列 $ S,\ T $ に対し、関数 $ f(S,\ T) $ を以下のように定めます。

- $ S $ に対し以下の操作を繰り返して $ T $ と等しくすることを考える。このとき行う操作のコストの和として考えられる最小の値が $ f(S,\ T) $ である。
  
  
  - $ S_i $ を ($ 0 $ から $ 1 $、もしくは $ 1 $ から $ 0 $ に) 変更する。この操作のコストは、変更の直前に $ S_j\ \neq\ T_j\ (1\ \leq\ j\ \leq\ N) $ であったような整数 $ j $ の個数を $ D $ として、$ D\ \times\ C_i $ である。

$ 0,\ 1 $ からなる長さ $ N $ の異なる $ 2 $ つの数列の組 $ (S,\ T) $ は $ 2^N\ \times\ (2^N\ -\ 1) $ 通り考えられます。これらすべてに対する $ f(S,\ T) $ の和を $ 10^9+7 $ で割った余りを計算してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ C_1 $ $ C_2 $ $ \cdots $ $ C_N $

## 输出格式
$ f(S,\ T) $ の和を $ 10^9+7 $ で割った余りを出力せよ。

## 题目大意
### 题目描述：
对于两个长度为 $n$ 的 $\texttt{01}$ 序列 $S,T$ ，我们定义 $f(S,T)$ 为通过以下操作将 $S$ 修改为 $T$ 的最小代价和: 选择一个 $S$ 中的二进制位 $S_{i}$ ，然后改变 $S_{i}$ 的 $\texttt{01}$ 状态，代价为 $D \times C_{i}$，其中 $D$ 是此次操作前满足 $S_{j}\ne T_{j}$ 的整数 $j$ 的数量，$C_{i}$ 是一个给定的序列中的一个值。

求当 $S$ 取 $2^n$ 种不同的状态，$T$ 取 $2^n$ 种不同的状态时，$f(S,T)$ 的和对 $1000000007$ 取模的结果。

### 输入格式：
第一行一个整数 $n$

第二行 $n$ 个整数 $C_{i}$

### 输出格式:
一行一个整数，表示答案

### 说明/提示:
$1 \le n \le 200000 , 1 \le C_{i} \le 10^9 $

```input1
1
1000000000
```

```output1
999999993
```

```input2
2
5 8
```

```output2
124
```

```input3
5
52 67 72 25 79
```

```output3
269312
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ C_i\ \leq\ 10^9 $
- 入力は全て整数である

### Sample Explanation 1

$ 0,\ 1 $ からなる長さ $ 1 $ の異なる $ 2 $ つの数列の組 $ (S,\ T) $ は以下の $ 2 $ 通りが考えられます。 - $ S\ =\ (0),\ T\ =\ (1): $ $ S_1 $ を $ 1 $ に変更することでコスト $ 1000000000 $ で $ S\ =\ T $ とできるため、$ f(S,\ T)\ =\ 1000000000 $ です。 - $ S\ =\ (1),\ T\ =\ (0): $ $ S_1 $ を $ 0 $ に変更することでコスト $ 1000000000 $ で $ S\ =\ T $ とできるため、$ f(S,\ T)\ =\ 1000000000 $ です。 これらの和は $ 2000000000 $ であり、これを $ 10^9+7 $ で割った余りは $ 999999993 $ です。

### Sample Explanation 2

$ 0,\ 1 $ からなる長さ $ 2 $ の異なる $ 2 $ つの数列の組 $ (S,\ T) $ は $ 12 $ 通り存在し、例えば以下のものが考えられます。 - $ S\ =\ (0,\ 1),\ T\ =\ (1,\ 0) $ この場合、$ 1 $ 回目の操作で $ S_1 $ を $ 1 $ に変更し、$ 2 $ 回目の操作で $ S_2 $ を $ 0 $ に変更するとき、操作のコストの和は $ 5\ \times\ 2\ +\ 8\ =\ 18 $ です。これより小さいコストで $ S\ =\ T $ とすることはできないので、$ f(S,\ T)\ =\ 18 $ です。

