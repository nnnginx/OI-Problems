## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc226/tasks/abc226_h

$ N $ 個の連続確率変数 $ X_1,X_2,\dots,X_N $ があり、 $ X_i $ は $ \lbrack\ L_i,\ R_i\ \rbrack $ の範囲を取る連続一様分布に従います。  
 $ N $ 個の確率変数のうち大きい方から $ K $ 番目の値の期待値を $ E $ とします。注記に述べるように $ E\ \bmod\ {998244353} $ を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ L_1 $ $ R_1 $ $ L_2 $ $ R_2 $ $ \vdots $ $ L_N $ $ R_N $

## 输出格式
$ E\ \bmod\ {998244353} $ を出力せよ。

## 题目大意
有 $n$ 个连续随机变量 $X_1, X_2, \dots, X_n$，$X_i$ 在 $[l_i, r_i]$ 上连续均匀分布。令 $E$ 为这 $n$ 个变量的第 $k$ 大值的期望，请求得 $E$ 在模 $998244353$ 意义下的值。

在本题的限制下，我们可以证明 $E$ 总能被表示为 $p / q$ 的形式，其中 $p, q$ 为 $< 998244353$ 的非负整数，且 $q$ 不为 $0$。你需要输出的即为一个 $< 998244353$ 的非负整数 $r$，满足 $qr \equiv p \pmod{998244353}$。

$1\le n\le 50,\ 1\le k\le n, \ 0\le l_i < r_i \le 100$，任意 $l_i, r_i$ 为整数。

```input1
1 1
0 2
```

```output1
1
```

```input2
2 2
0 2
1 3
```

```output2
707089751
```

```input3
10 5
35 48
44 64
47 59
39 97
36 37
4 91
38 82
20 84
38 50
39 69
```

```output3
810056397
```

## 提示
### 注記

この問題で $ E $ は必ず有理数になることが証明できます。また、この問題の制約下では、$ E $ を既約分数 $ \frac{y}{x} $ で表したときに $ x $ が $ 998244353 $ で割り切れないことが保証されます。  
 このとき $ xz\ \equiv\ y\ \pmod{998244353} $ を満たすような $ 0 $ 以上 $ 998244352 $ 以下の整数 $ z $ が一意に定まります。この $ z $ を $ E\ \bmod\ {998244353} $ として出力してください。

### 制約

- $ 1\ \leq\ N\ \leq\ 50 $
- $ 1\ \leq\ K\ \leq\ N $
- $ 0\ \leq\ L_i\ \lt\ R_i\ \leq\ 100 $
- 入力はすべて整数である。

### Sample Explanation 1

$ \lbrack\ 0,\ 2\ \rbrack $ 上の連続一様分布に従う確率変数の値の期待値が求める答えです。よって $ 1 $ を出力します。

### Sample Explanation 2

答えを有理数で表すと $ \frac{23}{24} $ になります。$ 707089751\ \times\ 24\ \equiv\ 23\ \pmod{998244353} $ なので $ 707089751 $ を出力します。

