# AT_abc265_f [ABC265F] Manhattan Cafe

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc265/tasks/abc265_f

$ N $ 次元空間上の $ 2 $ 点 $ x=(x_1,\ x_2,\ \dots,\ x_N) $, $ y\ =\ (y_1,\ y_2,\ \dots,\ y_N) $ のマンハッタン距離 $ d(x,y) $ は次の式で定義されます。

$ \displaystyle\ d(x,y)=\sum_{i=1}^n\ \vert\ x_i\ -\ y_i\ \vert $ 

また、座標成分 $ x_1,\ x_2,\ \dots,\ x_N $ がすべて整数であるような点 $ x=(x_1,\ x_2,\ \dots,\ x_N) $ を格子点と呼びます。

$ N $ 次元空間上の格子点 $ p=(p_1,\ p_2,\ \dots,\ p_N) $, $ q\ =\ (q_1,\ q_2,\ \dots,\ q_N) $ が与えられます。  
$ d(p,r)\ \leq\ D $ かつ $ d(q,r)\ \leq\ D $ であるような格子点 $ r $ としてあり得るものは全部で何個ありますか？答えを $ 998244353 $ で割ったあまりを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ D $ $ p_1 $ $ p_2 $ $ \dots $ $ p_N $ $ q_1 $ $ q_2 $ $ \dots $ $ q_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
1 5
0
3
```

### 输出 #1

```
8
```

## 输入输出样例 #2

### 输入 #2

```
3 10
2 6 5
2 1 2
```

### 输出 #2

```
632
```

## 输入输出样例 #3

### 输入 #3

```
10 100
3 1 4 1 5 9 2 6 5 3
2 7 1 8 2 8 1 8 2 8
```

### 输出 #3

```
145428186
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ 0\ \leq\ D\ \leq\ 1000 $
- $ -1000\ \leq\ p_i,\ q_i\ \leq\ 1000 $
- 入力される値はすべて整数

### Sample Explanation 1

$ N=1 $ の場合は $ 1 $ 次元空間、すなわち数直線上の点に関する問題になります。 条件を満たす点は $ -2,-1,0,1,2,3,4,5 $ の $ 8 $ 個です。