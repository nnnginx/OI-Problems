# AT_joi2020_yo1b_a 試験 (Exam)

## 题目描述

[problemUrl]: https://atcoder.jp/contests/joi2020yo1b/tasks/joi2020_yo1b_a

JOI 君は情報の試験を $ 3 $ 回受けた．試験の点数はすべて $ 0 $ 以上 $ 100 $ 以下の整数である．

JOI 君の成績は $ 3 $ 回の試験の点数のうち高い方から $ 2 $ つを足し合わせた合計によって決まる．

$ 3 $ 回の試験の点数 $ A,\ B,\ C $ が与えられたとき，$ 3 $ 回の試験の点数のうち高い方から $ 2 $ つを足し合わせた合計を出力するプログラムを作成せよ．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ A $ $ B $ $ C $

## 输出格式

$ 3 $ 回の試験の点数のうち高い方から $ 2 $ つを足し合わせた合計を $ 1 $ 行で出力せよ．

## 输入输出样例 #1

### 输入 #1

```
70 80 90
```

### 输出 #1

```
170
```

## 输入输出样例 #2

### 输入 #2

```
70 100 70
```

### 输出 #2

```
170
```

## 输入输出样例 #3

### 输入 #3

```
70 70 70
```

### 输出 #3

```
140
```

## 说明/提示

### 制約

- $ 0\ \leqq\ A\ \leqq\ 100 $．
- $ 0\ \leqq\ B\ \leqq\ 100 $．
- $ 0\ \leqq\ C\ \leqq\ 100 $．
- 入力はすべて整数である．

### Sample Explanation 1

点数は高い順に $ 90,\ 80,\ 70 $ であるから，求める和は $ 90\ +\ 80\ =\ 170 $ である．

### Sample Explanation 2

点数は高い順に $ 100,\ 70,\ 70 $ であるから，求める和は $ 100\ +\ 70\ =\ 170 $ である．