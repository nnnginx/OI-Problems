# AT_abc100_c [ABC100C] *3 or /2

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc100/tasks/abc100_c

AtCoder Beginner Contest 100 の開催にともなって, AtCoder 社では長さ $ N $ の数列 $ a\ = ${$ a_1,\ a_2,\ a_3,\ ...,\ a_N $} が飾られることになった.   
 社員のすぬけ君は, この数列で遊んでみようと思った.

具体的には, 以下の操作をできるだけ多くの回数繰り返そうと思った.

> $ 1\ \leq\ i\ \leq\ N $ を満たす全ての $ i $ に対して, それぞれ「$ a_i $ の値を $ 2 $ で割る」「$ a_i $ の値を $ 3 $ 倍する」のどちらかを行う. ただし, 全ての $ i $ に対して $ 3 $ 倍することはできず, 操作後の $ a_i $ の値は整数でなければならない.

最大で何回の操作が可能か, 求めなさい.

## 输入格式

入力は以下の形式で標準入力から与えられる.

> $ N $ $ a_1 $ $ a_2 $ $ a_3 $ $ ... $ $ a_N $

## 输出格式

すぬけ君が行える最大の操作回数を出力しなさい.

## 输入输出样例 #1

### 输入 #1

```
3
5 2 4
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
4
631 577 243 199
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
10
2184 2126 1721 1800 1024 2528 3360 1945 1280 1776
```

### 输出 #3

```
39
```

## 说明/提示

### 制約

- $ N $ は $ 1 $ 以上 $ 10\ 000 $ 以下の整数
- $ a_i $ は $ 1 $ 以上 $ 1\ 000\ 000\ 000 $ 以下の整数

### Sample Explanation 1

最初, 数列は $ {5,\ 2,\ 4} $ であるが, 以下のように操作すれば $ 3 $ 回の操作を行うことができる. - 最初に, $ a_1 $ を $ 3 $ 倍し, $ a_2 $ を $ 3 $ 倍し, $ a_3 $ を $ 2 $ で割る. すると数列は $ {15,\ 6,\ 2} $ となる. - 次に, $ a_1 $ を $ 3 $ 倍し, $ a_2 $ を $ 2 $ で割り, $ a_3 $ を $ 3 $ 倍する. すると数列は $ {45,\ 3,\ 6} $ となる. - 最後に, $ a_1 $ を $ 3 $ 倍し, $ a_2 $ を $ 3 $ 倍し, $ a_3 $ を $ 2 $ で割る. すると数列は $ {135,\ 9,\ 3} $ となる.

### Sample Explanation 2

全ての要素が奇数なので, 操作はできない. よって答えは $ 0 $ である.