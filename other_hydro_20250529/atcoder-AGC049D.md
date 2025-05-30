## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc049/tasks/agc049_d

整数 $ N $ と $ M $ が与えられます． 長さ $ N $ の非負整数列 $ (A_1,A_2,\ldots,A_N) $ であって，次の条件を満たすものの個数を$ \bmod\ (10^9+7) $ で求めてください．

- $ A_1+A_2+\ldots\ +A_N\ =\ M $
- すべての $ i $ ($ 2\ \leq\ i\ \leq\ N-1 $) について，$ 2\ A_i\ \leq\ A_{i-1}\ +\ A_{i+1} $

## 输入格式
入力は以下の形式で標準入力から与えられる．

> $ N $ $ M $

## 输出格式
条件を満たす数列の個数を$ \bmod\ (10^9+7) $ で出力せよ．

## 题目大意
给定整数 $N$ 和 $M$，问有多少个长为 $N$ 的非负整数数列 $A$，满足以下条件：

- $A_1+A_2+\ldots+A_N = M$
- 对任意 $i(2 \leq i \leq N-1)$ ，都有 $2A_i \leq A_{i-1} + A_{i+1}$

答案对 $10^9+7$ 取模。

```input1
3 3
```

```output1
7
```

```input2
10 100
```

```output2
10804516
```

```input3
10000 100000
```

```output3
694681734
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ M\ \leq\ 10^5 $
- 入力はすべて整数である．

### Sample Explanation 1

以下の $ 7 $ 個の数列が条件を満たします． - $ 0,0,3 $ - $ 0,1,2 $ - $ 1,0,2 $ - $ 1,1,1 $ - $ 2,0,1 $ - $ 2,1,0 $ - $ 3,0,0 $

