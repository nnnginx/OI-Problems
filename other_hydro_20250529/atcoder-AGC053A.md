## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc053/tasks/agc053_a

長さ $ N $ の文字列 $ S $ があります。$ S $ の各文字は `<` または `>` です。

要素数 $ N+1 $ の非負整数列 $ X_0,X_1,\ldots,X_N $ は、すべての $ 1\ \leq\ i\ \leq\ N $ について次の条件を満たすとき *良い非負整数列* と呼ばれます。

- $ S_i $ が `<` のとき : $ X_{i-1}\ <\ X_i $
- $ S_i $ が `>` のとき : $ X_{i-1}\ >\ X_i $

良い非負整数列 $ A $ が与えられるので、この数列をできるだけ多くの良い非負整数列に分解してください。 つまり、正の整数 $ k $ および $ k $ 個の良い非負整数列 $ B_1,B_2,\ldots,\ B_k $ であって、次の条件を満たすもののうち、 $ k $ が最大のものを $ 1 $ つ求めてください。

- すべての $ 0\ \leq\ i\ \leq\ N $ について $ B_1,\ldots,B_k $ の $ i $ 項目の値の合計は $ A_i $ と等しい。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $ $ A_0 $ $ A_1 $ $ \cdots $ $ A_N $

## 输出格式
以下の形式で、標準出力に出力せよ。

> $ k $ $ B_{1,0} $ $ B_{1,1} $ $ \cdots $ $ B_{1,N} $ $ : $ $ B_{k,0} $ $ B_{k,1} $ $ \cdots $ $ B_{k,N} $

ここで、$ B_{i,j} $ は良い非負整数列 $ B_i $ の $ j $ 項目の値を表している。

## 题目大意
给定长为 $n$ 的字符串 $S$，其由 `<` 与 `>` 组成。

我们称一个长度为 $n+1$ 的非负整数序列 $x=(x_0,x_1,\dots,x_n)$ 是好的，当且仅当对于任意 $1\le i\le n$，有：
- 若 $S_i$ 为 `<`，则 $x_{i-1} < x_i$；
- 若 $S_i$ 为 `>`，则 $x_{i-1} > x_i$；

给定一个好的非负整数序列 $A$，你需要将其拆分为尽可能多的好的非负整数序列。具体地说，你需要找到正整数 $k$ 以及 $k$ 个好的非负整数序列 $B_1,B_2,\dots,B_k$，满足对于任意 $0\le i \le n$，$\sum_{j=1}^k B_{j,i} = A_i$。

你需要最大化 $k$ 的值。输出这个值，以及你所构造的 $k$ 个长度为 $n + 1$ 的串。   
如果有多组解，输出任意一组即可。

$1\le n \le 100, 0\le a_i\le 10^4$。

```input1
3
<><
3 8 6 10
```

```output1
2
1 5 4 7
2 3 2 3
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ 0\ \leq\ A_i\ \leq\ 10^4 $
- $ S $ は `<` と `>` からなる長さ $ N $ の文字列である。
- $ A $ は良い非負整数列である。特に、要素数は $ N+1 $ である。