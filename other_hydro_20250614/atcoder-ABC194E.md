## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc194/tasks/abc194_e

$ \mathrm{mex}(x_1,\ x_2,\ x_3,\ \dots,\ x_k) $ を、$ x_1,\ x_2,\ x_3,\ \dots,\ x_k $ に含まれない最小の非負整数と定義します。  
 長さ $ N $ の整数列 $ A\ =\ (A_1,\ A_2,\ A_3,\ \dots,\ A_N) $ が与えられます。  
 $ 0\ \le\ i\ \le\ N\ -\ M $ を満たす全ての整数 $ i $ について $ \mathrm{mex}(A_{i\ +\ 1},\ A_{i\ +\ 2},\ A_{i\ +\ 3},\ \dots,\ A_{i\ +\ M}) $ を計算したとき、この $ N\ -\ M\ +\ 1 $ 個の値のうちの最小値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ A_1 $ $ A_2 $ $ A_3 $ $ \cdots $ $ A_N $

## 输出格式
答えを出力せよ。

## 题目大意
- 给你一个长度为 $N$ 的序列 $A$，求 $A$ 中所有长度为 $M$ 的连续子序列中，最小的 $\operatorname{mex}$ 值（定义 $\operatorname{mex}$ 为序列中最小未出现的自然数）。
- $1\le M\le N\le 15\times 10^5,\ 0\le A_i< N$。

@[hellolin](/user/751017) 译

```input1
3 2
0 0 1
```

```output1
1
```

```input2
3 2
1 1 1
```

```output2
0
```

```input3
3 2
0 1 0
```

```output3
2
```

```input4
7 3
0 0 1 2 0 1 0
```

```output4
2
```

## 提示
### 制約

- $ 1\ \le\ M\ \le\ N\ \le\ 1.5\ \times\ 10^6 $
- $ 0\ \le\ A_i\ \lt\ N $
- 入力に含まれる値は全て整数

### Sample Explanation 1

\- $ i\ =\ 0 $ のとき : $ \mathrm{mex}(A_{i\ +\ 1},\ A_{i\ +\ 2})\ =\ \mathrm{mex}(0,\ 0)\ =\ 1 $ - $ i\ =\ 1 $ のとき : $ \mathrm{mex}(A_{i\ +\ 1},\ A_{i\ +\ 2})\ =\ \mathrm{mex}(0,\ 1)\ =\ 2 $ よって $ 1 $ と $ 2 $ のうちの最小値である $ 1 $ が答えです。

### Sample Explanation 2

\- $ i\ =\ 0 $ のとき : $ \mathrm{mex}(A_{i\ +\ 1},\ A_{i\ +\ 2})\ =\ \mathrm{mex}(1,\ 1)\ =\ 0 $ - $ i\ =\ 1 $ のとき : $ \mathrm{mex}(A_{i\ +\ 1},\ A_{i\ +\ 2})\ =\ \mathrm{mex}(1,\ 1)\ =\ 0 $ となります。

### Sample Explanation 3

\- $ i\ =\ 0 $ のとき : $ \mathrm{mex}(A_{i\ +\ 1},\ A_{i\ +\ 2})\ =\ \mathrm{mex}(0,\ 1)\ =\ 2 $ - $ i\ =\ 1 $ のとき : $ \mathrm{mex}(A_{i\ +\ 1},\ A_{i\ +\ 2})\ =\ \mathrm{mex}(1,\ 0)\ =\ 2 $ となります。

