## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc126/tasks/arc126_f

$ N $ 項からなる正整数列 $ X\ =\ (X_1,\ X_2,\ \ldots,\ X_N) $ が与えられます。

正の整数 $ K $ に対して、整数の組 $ (a,b,c) $ のうちで以下の条件がすべて成り立つものの個数を $ f(K) $ と書くことにします。

- $ 1\leq\ c\ \leq\ K $
- $ 0\leq\ a\ <\ c $ かつ $ 0\leq\ b\ <\ c $
- 各 $ i $ に対して $ aX_i\ +\ b $ を $ c $ で割った余りを $ Y_i $ とするとき、$ Y_1\ <\ Y_2\ <\ \cdots\ <\ Y_N $ が成り立つ。

極限 $ \displaystyle\ \lim_{K\to\infty}\ \frac{f(K)}{K^3} $ が存在することが証明できます。 この値を $ \mod\ 998244353 $ で求めてください（注記参照）。

## 输入格式
入力は以下の形式で標準入力から与えられます。

> $ N $ $ X_1 $ $ X_2 $ $ \ldots $ $ X_N $

## 输出格式
$ \displaystyle\ \lim_{K\to\infty}\ \frac{f(K)}{K^3} $ を $ \mod\ 998244353 $ で出力してください。

## 题目大意
给定长度为 $N$ 的正整数序列 $X_1,X_2,\cdots,X_n$。

对于正整数 $K$，$F(K)$ 表示满足以下条件的三元组 $(a,b,c)$ 的个数：

- $c\in[1,K],a,b\in[0,c)$。

- $aX_i+b$ 模 $c$ 单调递增。

求 $\lim\limits_{K\to \infty}\frac{F(K)}{K^3} \bmod 998244353$。

translated by syzf2222

```input1
3
3 1 2
```

```output1
291154603
```

```input2
3
5 9 2
```

```output2
832860616
```

```input3
2
2 3
```

```output3
166374059
```

```input4
4
4 5 3 2
```

```output4
0
```

## 提示
### 注記

求める極限は必ず有理数となることが証明できます。またこの問題の制約下では、その値を互いに素な $ 2 $ つの整数 $ P,\ Q $ を用いて $ \frac{P}{Q} $ と表したとき、$ R\times\ Q\equiv\ P\pmod{998244353} $ かつ $ 0\leq\ R\ <\ 998244353 $ を満たす整数 $ R $ がただ一つ存在することが証明できます。この $ R $ を求めてください。

### 制約

- $ 2\leq\ N\leq\ 10^3 $
- $ X_i $ は正の整数で、$ \sum_{i=1}^N\ X_i\ \leq\ 5\times\ 10^5 $ を満たす
- $ i\neq\ j $ ならば $ X_i\neq\ X_j $

### Sample Explanation 1

\- 例えば $ (a,b,c)\ =\ (3,5,7) $ とすると、$ Y_1\ =\ 0 $, $ Y_2\ =\ 1 $, $ Y_3\ =\ 4 $ となり、$ Y_1\ <\ Y_2\ <\ Y_3 $ が成り立ちます。 - $ f(1)\ =\ 0 $, $ f(2)\ =\ 0 $, $ f(3)\ =\ 1 $, $ f(4)\ =\ 2 $, $ f(5)\ =\ 5 $ が成り立ちます。 - $ \displaystyle\ \lim_{K\to\infty}\ \frac{f(K)}{K^3}\ =\ \frac{1}{24} $ が成り立ちます。

### Sample Explanation 2

$ \displaystyle\ \lim_{K\to\infty}\ \frac{f(K)}{K^3}\ =\ \frac{55}{1008} $ が成り立ちます。

### Sample Explanation 3

$ \displaystyle\ \lim_{K\to\infty}\ \frac{f(K)}{K^3}\ =\ \frac{1}{6} $ が成り立ちます。

### Sample Explanation 4

$ \displaystyle\ \lim_{K\to\infty}\ \frac{f(K)}{K^3}\ =\ 0 $ が成り立ちます。

