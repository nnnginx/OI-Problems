## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc041/tasks/agc041_d

コンテストで使う $ N $ 問の問題がジャッジに選ばれ、各問に配点を付ける段階になりました。

問題 $ i $ の配点 $ A_i $ は、$ 1 $ 以上 $ N $ 以下の整数でなければなりません。 また、すでに問題は難易度順に並んでおり、$ A_1\ \le\ A_2\ \le\ \ldots\ \le\ A_N $ でなければなりません (複数問の配点が同じになるのは構いませんが)。

ICPC のファンであるあなたは、解いた問題数が多い参加者ほど上位となってほしいと考えています。 この理由から、任意の $ k $ ($ 1\ \le\ k\ \le\ N-1 $) に対して、任意の $ k $ 問の配点の合計が任意の $ k+1 $ 問の配点の合計より真に小さくなるようにしたい、とあなたは考えています。

このような配点の付け方は何通りあるでしょうか？この数を与えられた素数 $ M $ で割った余りを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $

## 输出格式
配点の付け方の数を $ M $ で割った余りを出力せよ。

## 题目大意
- 有 $n$ 道还未赋分的题目，你需要给这 $n$ 道题目赋分。
- 设第 $i$ 道题目的分数为 $A_i$。给题目赋分的方案需要满足：
  - 对于任意 $i \in [2, n]$，$A_{i-1} \leq A_{i}$。
  - 对于任意 $i \in [1, n]$，$1 \leq A_{i} \leq n$。
  - 对于任意一个大小为 $k$（$1 \leq k < n$）的题目子集 $S$ 和任意一个大小为 $k+1$ 的题目子集 $T$，需要满足：$\sum_{x \in S}A_x < \sum_{x\in T}A_x$。
- 你需要计算，有多少种给题目赋分的方案，使得能满足上述三个条件。请求出答案对 $M$ 取模的结果。

```input1
2 998244353
```

```output1
3
```

```input2
3 998244353
```

```output2
7
```

```input3
6 966666661
```

```output3
66
```

```input4
96 925309799
```

```output4
83779
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 5000 $
- $ 9\ \times\ 10^8\ <\ M\ <\ 10^9 $
- $ M $ は素数である。
- 入力中のすべての値は整数である。

### Sample Explanation 1

可能な配点の付け方は $ (1,\ 1) $, $ (1,\ 2) $, $ (2,\ 2) $ です。

### Sample Explanation 2

可能な配点の付け方は $ (1,\ 1,\ 1) $, $ (1,\ 2,\ 2) $, $ (1,\ 3,\ 3) $, $ (2,\ 2,\ 2) $, $ (2,\ 2,\ 3) $, $ (2,\ 3,\ 3) $, $ (3,\ 3,\ 3) $ です。

