# AT_arc162_e [ARC162E] Strange Constraints

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc162/tasks/arc162_e

$ 1 $ 以上 $ N $ 以下の整数からなる長さ $ N $ の数列 $ A=(A_1,A_2,\ldots,A_N) $ が与えられます。

$ 1 $ 以上 $ N $ 以下の整数からなる長さ $ N $ の数列 $ B=(B_1,B_2,\ldots,B_N) $ のうち、全ての $ i=1,2,\ldots,N $ に対して以下の条件を満たすものの個数を $ 998244353 $ で割ったあまりを求めてください。

- $ B $ の中に含まれる $ i $ の個数は $ A_i $ 個以下
- $ B $ の中に含まれる $ B_i $ の個数は $ A_i $ 個以下

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
1 2 3
```

### 输出 #1

```
10
```

## 输入输出样例 #2

### 输入 #2

```
4
4 4 4 4
```

### 输出 #2

```
256
```

## 输入输出样例 #3

### 输入 #3

```
5
1 1 1 1 1
```

### 输出 #3

```
120
```

## 输入输出样例 #4

### 输入 #4

```
14
6 5 14 3 6 7 3 11 11 2 3 7 8 10
```

### 输出 #4

```
628377683
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 500 $
- $ 1\ \leq\ A_i\ \leq\ N $
- 入力される数値は全て整数
 
### Sample Explanation 1

条件を満たす数列は以下の $ 10 $ 個です。 - $ (1,2,2) $ - $ (1,2,3) $ - $ (1,3,2) $ - $ (1,3,3) $ - $ (2,1,3) $ - $ (2,3,1) $ - $ (2,3,3) $ - $ (3,1,2) $ - $ (3,2,1) $ - $ (3,2,2) $

### Sample Explanation 2

条件を満たす数列は、$ 1 $ 以上 $ 4 $ 以下の整数からなる長さ $ 4 $ の数列全てで、その個数は $ 4^4=256 $ 個です。

### Sample Explanation 3

条件を満たす数列は、$ (1,2,3,4,5) $ を並び替えて得られる数列全てで、その個数は $ 5!=120 $ 個です。

### Sample Explanation 4

個数を $ 998244353 $ で割ったあまりを出力してください。