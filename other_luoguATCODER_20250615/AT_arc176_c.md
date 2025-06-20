# AT_arc176_c [ARC176C] Max Permutation

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc176/tasks/arc176_c

$ (1,2,\dots,N) $ の順列 $ P=(P_1,P_2,\dots,P_N) $ のうち、以下の条件を全て満たすものの個数を $ 998244353 $ で割ったあまりを出力してください。

- $ \max(P_{A_i},P_{B_i})\ =\ C_i\ (1\ \le\ i\ \le\ M) $

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ A_1 $ $ B_1 $ $ C_1 $ $ A_2 $ $ B_2 $ $ C_2 $ $ \vdots $ $ A_M $ $ B_M $ $ C_M $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4 2
1 2 4
2 3 2
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
6 3
1 4 3
2 5 6
3 4 2
```

### 输出 #2

```
8
```

## 输入输出样例 #3

### 输入 #3

```
20 17
9 16 13
5 14 20
15 20 14
5 13 17
18 20 14
14 20 20
6 13 11
12 16 19
2 15 10
6 17 11
7 18 7
8 18 12
8 16 13
6 16 13
2 18 10
9 10 15
7 14 20
```

### 输出 #3

```
1209600
```

## 说明/提示

### 制約

- $ 2\ \le\ N\ \le\ 2\ \times\ 10^5 $
- $ 1\ \le\ M\ \le\ 2\ \times\ 10^5 $
- $ 1\ \le\ A_i\ <\ B_i\ \le\ N $
- $ 1\ \le\ C_i\ \le\ N $
- $ i\ \neq\ j $ ならば $ (A_i,B_i)\ \neq\ (A_j,B_j) $
 
### Sample Explanation 1

条件を満たす $ P $ は $ (4,1,2,3),(4,2,1,3) $ の $ 2 $ 個です。