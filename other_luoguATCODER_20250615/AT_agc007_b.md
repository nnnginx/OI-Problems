# AT_agc007_b [AGC007B] Construct Sequences

## 题目描述

# 题意简述
给你一段长度为 $n$ 的数列 $P_1,P_2,\dots,P_n$。

让你构造两个新的数列 $a$ 与 $b$，且满足：
1.    $1<a_i,b_i<10^9$
2.    $2\le n\le 20,000$
3.    $a_1<a_2<\dots<a_n$
4.    $b_1>b_2>\dots>b_n$
5.    $a_{p_1}+b_{p_1}<a_{p_2}+b_{p_2}<\dots<a_{p_n}+b_{p_n}$

求出满足条件的数列 $a,b$。

## 输入格式

两行，第一行为 $n$，第二行为数列 $P$。

## 输出格式

两行，第一行为数列 $a$，第二行为数列 $b$。

## 输入输出样例 #1

### 输入 #1

```
2
1 2
```

### 输出 #1

```
1 4
5 4
```

## 输入输出样例 #2

### 输入 #2

```
3
3 2 1
```

### 输出 #2

```
1 2 3
5 3 1
```

## 输入输出样例 #3

### 输入 #3

```
3
2 3 1
```

### 输出 #3

```
5 10 100
100 10 1
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 20,000 $
- $ p $ は集合 {$ 1,\ 2,\ ...,\ N $} の要素を並び替えた順列である。

### Sample Explanation 1

$ a_1\ +\ b_1\ =\ 6 $ および $ a_2\ +\ b_2\ =\ 8 $ より、すべての条件が満たされています。