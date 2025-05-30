## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc150/tasks/abc150_d

長さ $ N $ の偶数からなる正の整数列 $ A=\ {a_1,a_2,...,a_N} $ と、整数 $ M $ が与えられます。

任意の $ k(1\ \leq\ k\ \leq\ N) $ に対して以下の条件を満たす正の整数 $ X $ を $ A $ の「半公倍数」と定義します。

- $ X=\ a_k\ \times\ (p+0.5) $ を満たす負でない整数 $ p $ が存在する。

$ 1 $ 以上 $ M $ 以下の整数のうちの $ A $ の半公倍数の個数を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ a_1 $ $ a_2 $ $ ... $ $ a_N $

## 输出格式
$ 1 $ 以上 $ M $ 以下の整数のうちの $ A $ の半公倍数の個数を出力せよ。

## 题目大意
给定一个 $N$ 个数的数组 $a_i$ ，求出满足对所有的 $a_i$ ，存在自然数 $p$，满足 $X=a_i\times(p+0.5)$ 的 $X$ 的个数，且 $X\in[1,M]$。  
保证所有的 $a_i$ 都是偶数。

```input1
2 50
6 10
```

```output1
2
```

```input2
3 100
14 22 40
```

```output2
0
```

```input3
5 1000000000
6 6 2 6 2
```

```output3
166666667
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ M\ \leq\ 10^9 $
- $ 2\ \leq\ a_i\ \leq\ 10^9 $
- $ a_i $ は偶数である。
- 入力は全て整数である。

### Sample Explanation 1

\- $ 15\ =\ 6\ \times\ 2.5 $ - $ 15\ =\ 10\ \times\ 1.5 $ - $ 45\ =\ 6\ \times\ 7.5 $ - $ 45\ =\ 10\ \times\ 4.5 $ より、$ 15,45 $ は $ A $ の半公倍数です。$ 1 $ 以上 $ 50 $ 以下の整数に他に $ A $ の半公倍数はないので、答えは $ 2 $ となります。

### Sample Explanation 2

答えが $ 0 $ の場合もあります。

