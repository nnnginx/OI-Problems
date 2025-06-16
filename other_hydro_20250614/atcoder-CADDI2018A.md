## 题目描述
[problemUrl]: https://atcoder.jp/contests/caddi2018b/tasks/caddi2018_a

$ N $ 個の $ 1 $ 以上の整数 $ a_1,\ a_2,\ ...,\ a_N $ があります． $ a_1,\ a_2,\ ...,\ a_N $ の値はわかりませんが，$ a_1\ \times\ a_2\ \times\ ...\ \times\ a_N\ =\ P $ がわかっています．

$ a_1,\ a_2,\ ...,\ a_N $ の最大公約数として考えられるもののうち，最も大きいものを求めてください．

## 输入格式
入力は以下の形式で標準入力から与えられる．

> $ N $ $ P $

## 输出格式
答えを出力せよ．

## 题目大意
给你 $2$ 个整数 $N,P$。

你需要构造一个有 $N$ 个数的整数序列 $a$，满足以下条件：

+ $\forall i=1,2,..,N,a_i\ge 1$

+ $\prod\limits_{i=1}^{N}a_i=P$

求 $\gcd\limits_{i=1}^{N}a_i$ 可能的最大值。

$1\le N,P\le 10^{12}$

```input1
3 24
```

```output1
2
```

```input2
5 1
```

```output2
1
```

```input3
1 111
```

```output3
111
```

```input4
4 972439611840
```

```output4
206
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^{12} $
- $ 1\ \leq\ P\ \leq\ 10^{12} $

### Sample Explanation 1

例えば $ a_1=2,\ a_2=6,\ a_3=2 $ の場合，最大公約数は $ 2 $ となります．

### Sample Explanation 2

$ a_i $ は正の整数なので，$ a_1\ =\ a_2\ =\ a_3\ =\ a_4\ =\ a_5\ =\ 1 $ 以外にはありえません．

