# AT_arc056_d [ARC056D] サケノミ

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc056/tasks/arc056_d

あなたは風変わりなバーに来ています。このバーでは、$ N $種類のドリンクがあり、あなたは初めに$ N $個のグラスを与えられます。$ i $番目のグラスは$ i $番目のドリンクに対応しており、$ i $番目のドリンクのみが注がれます。また、それぞれのドリンクに対し、美味しさ$ w_i $が定まっています。初めに、全てのグラスは空です。

それぞれのドリンクは、何回か決まった時刻に補充されます。 すなわち、 時間$ t_{i,j}(1≦j≦M_i) $に$ i $番目のグラスが空ならば、$ i $番目のグラスに$ i $番目のドリンクが注がれます。

あなたは、好きな奇数時刻に、全てのグラスに入っているドリンクを全て飲み干すことができます。一部のドリンクのみを飲む行為は禁止されています。 飲んだドリンクの美味しさの総和の最大値を求めるプログラムを書いてください。ただし、同じドリンクを複数回飲んだときも、美味しさは重複して計算されることに注意してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ w_1 $ ... $ w_N $ $ M_1 $ $ t_{1,1} $ ... $ t_{1,M_1} $ : $ M_N $ $ t_{N,1} $ ... $ t_{N,M_N} $

## 输出格式

$ 1 $行目に、美味しさの総和を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
2 5 -6
1 2
2 4 10
2 4 8
```

### 输出 #1

```
6
```

## 输入输出样例 #2

### 输入 #2

```
3
2 5 -6
2 2 8
2 4 10
2 4 10
```

### 输出 #2

```
3
```

## 输入输出样例 #3

### 输入 #3

```
3
3 5 -4
2 2 8
4 4 6 10 12
4 2 4 8 10
```

### 输出 #3

```
18
```

## 输入输出样例 #4

### 输入 #4

```
3
-2 -2 -2
2 2 8
4 4 6 10 12
4 2 4 8 10
```

### 输出 #4

```
0
```

## 说明/提示

### 制約

- $ 1\ ≦\ N\ ≦\ 5*10^5 $
- $ 2\ ≦\ t_{i,j}\ ≦\ 10^6 $
- $ t_{i,j}\ <\ t_{i,j+1} $
- $ t_{i,j} $は偶数である
- $ Σ\ M_i\ ≦\ 5*10^5 $
- $ 1\ ≦\ M_i $
- $ -10^9\ ≦\ w_i\ ≦\ 10^9 $

### 部分点

- $ t_{i,j}\ ≦\ 1,000 $ かつ $ N\ ≦\ 1,000 $ を満たすテストケース全てに正解した場合、部分点として$ 30 $点が与えられる。

### Sample Explanation 1

時刻$ 9 $と$ 11 $にグラスにあるドリンクを全て飲み干します。 時刻$ 9 $では、$ 3 $つ全てドリンクが注がれているため、美味しさ$ 2+5-6=1 $を得ます。 時刻$ 11 $では、$ 2 $番目のドリンクのみ注がれているため、美味しさ$ 5 $を得ます。合計$ 6 $となります。