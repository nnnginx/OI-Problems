## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc178/tasks/abc178_c

長さ $ N $ の整数の列 $ A_1,A_2,\ldots,A_N $ であって以下の条件をすべて満たすものはいくつありますか。

- $ 0\ \leq\ A_i\ \leq\ 9 $
- $ A_i=0 $ なる $ i $ が存在する。
- $ A_i=9 $ なる $ i $ が存在する。

ただし、答えはとても大きくなる可能性があるので、$ 10^9+7 $ で割った余りを出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式
答えを$ 10^9+7 $ で割った余りを出力せよ。

## 题目大意
有一个长为 $n$ 的数列 $a_1,a_2,...,a_n$ ，其中对于每个 $a_i$ 都有 $0≤a_i≤9$ ，并保证数列中至少有一个 $a_i$ 为 $0$ 且至少有一个 $a_i$ 为 $9$ 。输入 $n$ ，输出满足条件的序列的个数对 $10^9+7$ 取模之后的余数。

```input1
2
```

```output1
2
```

```input2
1
```

```output2
0
```

```input3
869121
```

```output3
2511445
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^6 $
- $ N $ は整数

### Sample Explanation 1

数列$ \{0,9\} $,$ \{9,0\} $の $ 2 $ つが条件をすべて満たします。

