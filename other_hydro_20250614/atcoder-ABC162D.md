## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc162/tasks/abc162_d

`R`, `G`, `B` のみからなる、長さ $ N $ の文字列 $ S $ があります。

以下の $ 2 $ つの条件をともに満たす組 $ (i,~j,~k)~(1\ \leq\ i\ <\ j\ <\ k\ \leq\ N) $ の数を求めてください。

- $ S_i\ \neq\ S_j $ かつ $ S_i\ \neq\ S_k $ かつ $ S_j\ \neq\ S_k $ である
- $ j\ -\ i\ \neq\ k\ -\ j $ である

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式
題意を満たす組の数を出力せよ。

## 题目大意
给你一个仅由 $R$，$G$，$B$ 三种字符组成的字符串，你需要找到所有满足要求的三元组 $(i,j,k)$。其中 $S_i \ne S_j$，$S_j \ne S_k$，$S_i \ne S_k$，$j-i \ne k-j$，$1 \le i < j < k \le N$。其中 $N$ 是指 $S$ 中字符的个数。输出满足条件的三元组个数。

```input1
4
RRGB
```

```output1
1
```

```input2
39
RBRBGRBGGBBRRGBBRRRBGGBRBGBRBGBRBBBGBBB
```

```output2
1800
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 4000 $
- $ S $ は `R`, `G`, `B` のみからなる、長さ $ N $ の文字列である

### Sample Explanation 1

組 $ (1,~3,~4) $ だけが $ 2 $ つの条件をともに満たします。組 $ (2,~3,~4) $ は、$ 1 $ つ目の条件は満たしますが $ 2 $ つ目の条件を満たさないので不適です。

