## 题目背景
译自 [XXVIII Olimpiada Informatyczna - III etap](https://sio2.mimuw.edu.pl/c/oi28-3/dashboard/) [Kolekcjoner Bajtemonów 2](https://szkopul.edu.pl/problemset/problem/yI8VISW680r7ktJAPvA5QPkl/statement/)。

试机题。

## 题目描述
给你 $n$ 个数对，你要进行 $n$ 次二选一，这样你就有了 $n$ 个数，最大化这 $n$ 个数的 $\gcd$。

## 输入格式
第一行一个正整数 $n$。

接下来 $n$ 行，每行两个整数，$a_i,b_i$。

## 输出格式
一行一个数：最大的 $\gcd$。

```input1
4
5 7
10 15
13 20
7 5

```

```output1
5
```

```input2
2
18900 22050
14700 17640

```

```output2
7350
```

```input3
见附件
```

```output3
2
```

## 提示
对于所有数据，$1\leq n\leq 10^6$，$1\leq a_i\leq 5\times 10^5$，$1\leq b_i<2^{63}$。

对于 $42pts$ 的数据，$n\leq 5000$。

