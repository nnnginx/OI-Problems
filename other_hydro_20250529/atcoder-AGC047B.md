## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc047/tasks/agc047_b

リマクは、文字列の先頭 $ 2 $ 文字のうち片方を取り除くことを繰り返し行えます。例えば、$ abcxyx\ \rightarrow\ acxyx\ \rightarrow\ cxyx\ \rightarrow\ cyx $ とすることができます。

$ N $ 個の相異なる文字列 $ S_1,\ S_2,\ \ldots,\ S_N $ が与えられます。$ N\ \cdot\ (N-1)\ /\ 2 $ 個のペア $ (S_i,\ S_j) $ のうち何個において、リマクは一方からもう一方を得ることができるでしょうか。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_N $

## 输出格式
リマクが一方の文字列からもう一方を得られるような非順序対 $ (S_i,\ S_j) $ ($ i\ \neq\ j $) の個数を出力せよ。

## 题目大意
hhoppitree 有 $n$ 个字符串，其中第 $i$ 个字符串为 $s_i$，他想知道在所有的整数对 $(i,j)(1\le i\ne j\le n)$ 中，有多少对整数对 $(i,j)$ 满足 $s_i$ 能通过进行若干次以下操作成为 $s_j$：

- 当 $|s_i|\ge2$ 时，删去 $s_i$ 的前两个字符中的任意一个字符。

```input1
3
abcxyx
cyx
abc
```

```output1
1
```

```input2
6
b
a
abc
c
d
ab
```

```output2
5
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 200\,000 $
- $ S_i $ は英小文字 `a` - `z` からなる。
- $ S_i\ \neq\ S_j $
- $ 1\ \leq\ |S_i| $
- $ |S_1|\ +\ |S_2|\ +\ \ldots\ +\ |S_N|\ \leq\ 10^6 $

### Sample Explanation 1

条件を満たすペアは $ (abcxyx,\ cyx) $ のみです。

### Sample Explanation 2

条件を満たすペアは $ (b,\ abc) $, $ (a,\ abc) $, $ (abc,\ c) $, $ (b,\ ab) $, $ (a,\ ab) $ の $ 5 $ 個です。

