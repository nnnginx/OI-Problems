# AT_arc169_f [ARC169F] Large DP Table

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc169/tasks/arc169_f

長さ $ N $ の整数列 $ A=(A_1,A_2,\cdots,A_N) $, $ B=(B_1,B_2,\cdots,B_N) $, $ X=(X_1,X_2,\cdots,X_N) $, $ Y=(Y_1,Y_2,\cdots,Y_N) $ が与えられます． ここで，$ A,B $ は以下の性質を満たしています．

- $ A_1=1 $
- $ B_1=2 $
- $ (A_1,A_2,\cdots,A_N,B_1,B_2,\cdots,B_N) $ は $ (1,2,\cdots,2N) $ の順列．
 
整数 $ d_{i,j} $ ($ 1\ \leq\ i,j\ \leq\ N $) を以下のように定義します．

- $ d_{1,1}=0 $
- $ (i,j)\ \neq\ (1,1) $ かつ $ A_i\ <\ B_j $ のとき: $ d_{i,j}=d_{i,j-1}+X_i $
- $ (i,j)\ \neq\ (1,1) $ かつ $ A_i\ >\ B_j $ のとき: $ d_{i,j}=d_{i-1,j}+Y_j $
 
$ \sum_{1\ \leq\ i\ \leq\ N}\sum_{1\ \leq\ j\ \leq\ N}d_{i,j} $ を $ 998244353 $ で割ったあまりを求めてください．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ N $ $ A_1 $ $ A_2 $ $ \cdots $ $ A_N $ $ B_1 $ $ B_2 $ $ \cdots $ $ B_N $ $ X_1 $ $ X_2 $ $ \cdots $ $ X_N $ $ Y_1 $ $ Y_2 $ $ \cdots $ $ Y_N $

## 输出格式

答えを出力せよ．

## 输入输出样例 #1

### 输入 #1

```
2
1 4
2 3
2 2
1 3
```

### 输出 #1

```
8
```

## 输入输出样例 #2

### 输入 #2

```
3
1 3 5
2 6 4
1 10 100
1000 10000 100000
```

### 输出 #2

```
108153
```

## 输入输出样例 #3

### 输入 #3

```
3
1 6 5
2 4 3
1 10 100
1000 10000 100000
```

### 输出 #3

```
333009
```

## 输入输出样例 #4

### 输入 #4

```
10
1 17 4 7 16 18 9 3 12 6
2 19 20 14 5 11 13 8 15 10
744280520 249168130 239276621 320064892 910500852 164832983 245532751 198319687 715892722 967824729
769431650 80707350 459924868 257261830 777045524 583882654 950300099 438099970 322288793 532405020
```

### 输出 #4

```
746075419
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 250000 $
- $ A_1=1 $
- $ B_1=2 $
- $ (A_1,A_2,\cdots,A_N,B_1,B_2,\cdots,B_N) $ は $ (1,2,\cdots,2N) $ の順列．
- $ 1\ \leq\ X_i\ \leq\ 10^9 $
- $ 1\ \leq\ Y_i\ \leq\ 10^9 $
- 入力される値はすべて整数．
 
### Sample Explanation 1

$ d_{i,j} $ の値は以下のようになります． - $ d_{1,1}=0 $ - $ d_{1,2}=d_{1,1}+X_1=0+2=2 $ - $ d_{2,1}=d_{1,1}+Y_1=0+1=1 $ - $ d_{2,2}=d_{1,2}+Y_2=2+3=5 $ よって求める答えは $ 0+2+1+5=8 $ になります．