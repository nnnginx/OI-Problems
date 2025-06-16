## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc116/tasks/arc116_d

整数 $ N $ , $ M $ が与えられます。 長さ $ N $ の整数列 $ A $ であって、以下の条件を満たすものの数を答えてください。

- $ 0\ \leq\ A_i\ \left(i\ =\ 1,\ 2,\ \ldots,\ N\right) $
- $ \sum_{i\ =\ 1}^{N}\ A_i\ =\ M $
- $ A_1 $ xor $ A_2 $ xor $ \cdots $ xor $ A_N\ =\ 0 $ （ここで xor はビットごとの排他的論理和を表す）

ただし、答えは非常に大きくなる場合があるので、 $ 998244353 $ で割った余りを答えてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $

## 输出格式
答えを出力せよ。

## 题目大意
给定 $n,m$，问有多少个长度为 $n$ 的序列 $a$ 满足：

1. $0\leq a_i$
2. $\sum_{i=1}^n a_i=m$
3. $a_1\bigoplus a_2\bigoplus a_3\cdots =0$

- $1\le n,m\le 5000$

```input1
5 20
```

```output1
475
```

```input2
10 5
```

```output2
0
```

```input3
3141 2718
```

```output3
371899128
```

## 提示
### 制約

- 入力は全て整数
- $ 1\ \leq\ N\ \leq\ 5000 $
- $ 1\ \leq\ M\ \leq\ 5000 $

### Sample Explanation 1

条件を満たす数列 $ A $ として、例えば以下のようなものが考えられます。 - $ A\ =\ \left(10,\ 0,\ 10,\ 0,\ 0\right) $ - $ A\ =\ \left(1,\ 2,\ 3,\ 7,\ 7\right) $

