## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc281/tasks/abc281_e

長さ $ N $ の整数列 $ A\ =\ (A_1,\ \dots,\ A_N) $ と整数 $ M,\ K $ が与えられます。  
 $ i\ =\ 1,\ \dots,\ N\ -\ M\ +\ 1 $ に対して、次の独立な問題を解いてください。

> $ M $ 個の整数 $ A_i,\ A_{i\ +\ 1},\ \dots,\ A_{i\ +\ M\ -\ 1} $ を昇順に並べ替えたときの先頭 $ K $ 個の値の総和を求めよ。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ K $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式
$ i\ =\ k $ のときの問題の答えを $ \mathrm{answer}_k $ として、次の形式で出力せよ。

> $ \mathrm{answer}_1 $ $ \mathrm{answer}_2 $ $ \ldots $ $ \mathrm{answer}_{N-M+1} $

## 题目大意
### 【题目描述】

给定一个序列 $A$，对于每个 $1 \le i \le N - M + 1$，将 $A_i A_{i + 1} \cdots A_{i + M - 1}$ **从小到大**排序后（不影响原序列），求出 $\displaystyle ans_i = \sum\limits_{j=i}^{i+k-1} A_j$。


### 【输入格式】

> $N, M, K\\ A_1 A_2 \cdots A_N$

### 【输出格式】

> $\mathrm{ans}_1 \mathrm{ans}_2 \cdots \mathrm{ans}_{N-M+1}$

### 【数据范围】

$1 \le K \le M \le N \le 2 \times 10^5$

$1 \le A_i \le 10^9$

```input1
6 4 3
3 1 4 1 5 9
```

```output1
5 6 10
```

```input2
10 6 3
12 2 17 11 19 8 4 3 6 20
```

```output2
21 14 15 13 13
```

## 提示
### 制約

- $ 1\ \leq\ K\ \leq\ M\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ 10^9 $
- 入力される値は全て整数
 
### Sample Explanation 1

\- $ i\ =\ 1 $ のとき、$ A_i,\ A_{i+1},\ A_{i+2},\ A_{i+3} $ を小さい順に並べると $ 1,\ 1,\ 3,\ 4 $ となり、小さい方から $ 3 $ 個の値の総和は $ 5 $ です。 - $ i\ =\ 2 $ のとき、$ A_i,\ A_{i+1},\ A_{i+2},\ A_{i+3} $ を小さい順に並べると $ 1,\ 1,\ 4,\ 5 $ となり、小さい方から $ 3 $ 個の値の総和は $ 6 $ です。 - $ i\ =\ 3 $ のとき、$ A_i,\ A_{i+1},\ A_{i+2},\ A_{i+3} $ を小さい順に並べると $ 1,\ 4,\ 5,\ 9 $ となり、小さい方から $ 3 $ 個の値の総和は $ 10 $ です。

