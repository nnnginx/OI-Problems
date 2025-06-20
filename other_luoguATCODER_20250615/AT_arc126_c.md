# AT_arc126_c [ARC126C] Maximize GCD

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc126/tasks/arc126_c

$ N $ 項からなる正整数列 $ A\ =\ (A_1,\ A_2,\ \ldots,\ A_N) $ が与えられます。あなたはこの数列に対して、次の操作を $ 0 $ 回以上 $ K $ 回以下行うことができます：

- $ i\in\ \{1,2,\ldots,N\} $ をひとつ選び、$ A_i $ に $ 1 $ を加える。

操作後の $ \gcd(A_1,\ A_2,\ \ldots,\ A_N) $ としてありうる最大値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられます。

> $ N $ $ K $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式

操作後の $ \gcd(A_1,\ A_2,\ \ldots,\ A_N) $ としてありうる最大値を出力してください。

## 输入输出样例 #1

### 输入 #1

```
3 6
3 4 9
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
3 4
30 10 20
```

### 输出 #2

```
10
```

## 输入输出样例 #3

### 输入 #3

```
5 12345
1 2 3 4 5
```

### 输出 #3

```
2472
```

## 说明/提示

### 制約

- $ 2\leq\ N\leq\ 3\times\ 10^5 $
- $ 1\leq\ K\leq\ 10^{18} $
- $ 1\ \leq\ A_i\leq\ 3\times\ 10^5 $

### Sample Explanation 1

例えば以下のようにして、$ \gcd(A_1,\ A_2,\ A_3)\ =\ 5 $ を実現できます。 - $ i\ =\ 1 $ に対して $ 2 $ 回、$ i\ =\ 2 $ に対して $ 1 $ 回、$ i=3 $ に対して $ 1 $ 回の操作を行う。合計の操作回数は $ 4 $ 回で、$ K=6 $ 以下である。 - 操作の結果、$ A_1\ =\ 5 $, $ A_2\ =\ 5 $, $ A_3\ =\ 10 $ となり、$ \gcd(A_1,\ A_2,\ A_3)\ =\ 5 $ である。

### Sample Explanation 2

操作を一度も行わないことで、$ \gcd(A_1,\ A_2,\ A_3)\ =\ 10 $ を実現できます。