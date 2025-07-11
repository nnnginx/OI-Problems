# AT_code_thanks_festival_2017_a Time Penalty

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-thanks-festival-2017/tasks/code_thanks_festival_2017_a

CODE THANKS FESTIVAL 2017 では、問題を $ 8 $ 問解きます。   
 コンテスト参加者であるイルカの $ i(1≦i≦8) $ 問目の解答状況が $ t_i $ で与えられます。

$ t_i\ >\ 0 $ の場合には、$ i $ 問目の問題をコンテスト開始 $ t_i $ 秒後に正解しています。   
 一方で、$ t_i\ =\ 0 $ の場合には、まだ正解していません。

コンテスト参加者の時間ペナルティは、最後に正解した問題に対する $ t_i $ に等しいです。   
 また、$ 1 $ 問も正解していない場合の時間ペナルティは $ 0 $ とします。

イルカの時間ペナルティを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ t_1 $ $ t_2 $ $ t_3 $ $ t_4 $ $ t_5 $ $ t_6 $ $ t_7 $ $ t_8 $

## 输出格式

イルカの時間ペナルティを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
240
600
1800
3600
4800
7200
10000
0
```

### 输出 #1

```
10000
```

## 输入输出样例 #2

### 输入 #2

```
10400
10300
10100
9800
9500
8500
7000
5000
```

### 输出 #2

```
10400
```

## 输入输出样例 #3

### 输入 #3

```
0
0
0
0
0
0
0
0
```

### 输出 #3

```
0
```

## 说明/提示

### 制約

- $ 0≦t_i≦10800\ (1≦i≦8) $
- $ t_i $ は整数である。

### Sample Explanation 1

イルカは $ 8 $ 問目を除いた $ 7 $ つの問題に正解しており、最後に正解したのは $ 7 $ 問目であるため、$ t_7\ =\ 10000 $ を出力します。

### Sample Explanation 2

逆順に問題を解いている場合もあります。