# AT_agc060_d [AGC060D] Same Descent Set

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc060/tasks/agc060_d

$ (1,2,\cdots,N) $ の順列のペア $ (P,Q)=((P_1,P_2,\cdots,P_N),(Q_1,Q_2,\cdots,Q_N)) $ であって，次の条件を満たすものの個数を $ 998244353 $ で割ったあまりを求めてください．

- すべての $ i $ ($ 1\ \leq\ i\ \leq\ N-1 $) について，以下のいずれかの条件が成り立つ．
  - $ P_i\ <\ P_{i+1} $ かつ $ Q_i\ <\ Q_{i+1} $
  - $ P_i\ >\ P_{i+1} $ かつ $ Q_i\ >\ Q_{i+1} $

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ N $

## 输出格式

答えを出力せよ．

## 输入输出样例 #1

### 输入 #1

```
2
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
3
```

### 输出 #2

```
10
```

## 输入输出样例 #3

### 输入 #3

```
4
```

### 输出 #3

```
88
```

## 输入输出样例 #4

### 输入 #4

```
10
```

### 输出 #4

```
286574791
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- 入力される数はすべて整数

### Sample Explanation 1

$ (P,Q)=((1,2),(1,2)) $ と $ (P,Q)=((2,1),(2,1)) $ の $ 2 $ つが条件を満たします．