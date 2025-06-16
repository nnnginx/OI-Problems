# AT_ddcc2020_final_c Smaller-Suffix-Free Sequences

## 题目描述

[problemUrl]: https://atcoder.jp/contests/ddcc2020-final/tasks/ddcc2020_final_c

数列 $ T\ =\ (T_1,\ \ldots,\ T_L) $ が smaller-suffix-free であるとは、 $ i\ =\ 2,\ 3,\ \ldots,\ L $ 全てについて、 数列 $ (T_i,\ T_{i+1},\ \ldots,\ T_L) $ が 辞書順で $ T $ よりも大きいことを指します。 たとえば $ (5) $ や $ (1,\ 1,\ 2,\ 3) $ はsmaller-suffix-freeであり、$ (3,\ 2,\ 1) $ や $ (2,\ 2) $ は smaller-suffix-free ではありません。

長さ $ N $ の数列 $ A\ =\ (A_1,\ \ldots,\ A_N) $ が与えられます。 各 $ i\ =\ 1,\ \ldots,\ N $ について、$ (A_i,\ A_{i+1},\ \ldots,\ A_j) $ が smaller-suffix-free であるような最大の $ j $ を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式

出力は $ N $ 行からなる。

$ i $ 行目には $ (A_i,\ A_{i+1},\ \ldots,\ A_j) $ が smaller-suffix-free であるような最大の $ j $ を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
6
3 2 1 1 2 3
```

### 输出 #1

```
1
2
6
6
6
6
```

## 输入输出样例 #2

### 输入 #2

```
3
10 10 10
```

### 输出 #2

```
1
2
3
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ 2\ \times\ 10^5\ (1\ \leq\ i\ \leq\ N) $

### Sample Explanation 1

$ A_1 $ から始まる smaller-suffix-free である 最長の連続する部分列は $ (A_1)\ =\ (3) $ です。したがって $ 1 $ 行目には $ 1 $ を出力します。 同様に、$ (A_2),\ (A_3,\ A_4,\ A_5,\ A_6),\ (A_4,\ A_5,\ A_6),\ (A_5,\ A_6),\ (A_6) $ がそれぞれ $ A_i\ (2\ \leq\ i\ \leq\ 6) $ から始まる smaller-suffix-free である最長の連続する部分列です。