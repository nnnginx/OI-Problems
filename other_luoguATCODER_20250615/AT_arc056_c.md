# AT_arc056_c [ARC056C] 部門分け

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc056/tasks/arc056_c

高橋くんのいる会社は$ N $人の社員からなる。社員$ i $と社員$ j $の間には、信頼度$ w_{i,j} $が定まっている。 おかげ様で会社はぐんぐん成長したため、$ N $人をいくつかの部門に分けることになった。ここで、部門分けのスコアを、(部門の数)\*$ K $-(異なる部門に属する$ 2 $人の間の信頼度の総和)と定める。 スコアの最大値を求めるプログラムを書いてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ w_{1,1} $ ... $ w_{1,N} $ : $ w_{N,1} $ ... $ w_{N,N} $

## 输出格式

$ 1 $行目に、スコアの最大値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 3
0 1 5
1 0 1
5 1 0
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
4 8
0 2 3 5
2 0 1 2
3 1 0 8
5 2 8 0
```

### 输出 #2

```
11
```

## 输入输出样例 #3

### 输入 #3

```
5 10
0 10 1 2 1
10 0 1 2 1
1 1 0 6 7
2 2 6 0 8
1 1 7 8 0
```

### 输出 #3

```
12
```

## 说明/提示

### 制約

- $ 1\ ≦\ N\ ≦\ 17 $
- $ i≠j $ のとき、 $ 1\ ≦\ w_{i,j}\ ≦\ 10^6 $
- $ w_{i,i}\ =\ 0 $
- $ w_{i,j}=w_{j,i} $
- $ 1\ ≦\ K\ ≦\ 10^6 $
- 入力はすべて整数である

### 部分点

- $ N\ ≦\ 9 $ を満たすテストケース全てに正解した場合、部分点として$ 40 $点が与えられる。
- $ N\ ≦\ 15 $ を満たすテストケース全てに正解した場合、部分点として追加で$ 40 $点が与えられる。

### Sample Explanation 1

社員$ 1 $と$ 3 $で$ 1 $つの部門、社員$ 2 $で$ 1 $つの部門を作ると、 部門の数は$ 2 $つ、異なる部門の間の$ 2 $人の信頼度の総和は$ 2 $なので、$ 2*3-2=4 $となる。 スコアを$ 4 $より大きくする方法はない。