# AT_relay2_h Akashic Records

## 题目描述

[problemUrl]: https://atcoder.jp/contests/cf17-relay-open/tasks/relay2_h

無限個の項からなる数列 $ a_1, $ $ a_2, $ $ … $ を考えます。はじめ、すべての項の値は $ 0 $ であり、この状態から $ Q $ 回の操作を続けて行います。$ i $ 回目の操作 $ (1\ <\ =\ i\ <\ =\ Q) $ は次の通りです。

- すべての正の整数 $ j $ に対し、$ a_{j\ ×\ m_i} $ の値に $ x_i $ を加える。

これらの $ Q $ 回の操作後の最も大きい項の値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ Q $ $ m_1 $ $ x_1 $ $ : $ $ m_Q $ $ x_Q $

## 输出格式

$ Q $ 回の操作後の最も大きい項の値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
2 10
3 -20
6 15
```

### 输出 #1

```
10
```

## 输入输出样例 #2

### 输入 #2

```
3
10 -3
50 4
100 -5
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
5
56 114834
72 -149861
100 190757
192 -132693
240 133108
```

### 输出 #3

```
438699
```

## 说明/提示

### 制約

- $ 1\ <\ =\ Q\ <\ =\ 299 $
- $ 2\ <\ =\ m_i\ <\ =\ 300 $
- $ -10^6\ <\ =\ x_i\ <\ =\ 10^6 $
- $ m_i $ はすべて異なる。
- 入力値はすべて整数である。

### Sample Explanation 1

数列の各項 $ a_1, $ $ a_2, $ $ … $ の値は以下のように変化します。 - 操作前: $ 0, $ $ 0, $ $ 0, $ $ 0, $ $ 0, $ $ 0, $ $ … $ - $ 1 $ 回目の操作後: $ 0, $ $ 10, $ $ 0, $ $ 10, $ $ 0, $ $ 10, $ $ … $ - $ 2 $ 回目の操作後: $ 0, $ $ 10, $ $ -20, $ $ 10, $ $ 0, $ $ -10, $ $ … $ - $ 3 $ 回目の操作後: $ 0, $ $ 10, $ $ -20, $ $ 10, $ $ 0, $ $ 5, $ $ … $ すべての操作後の最も大きい項の値は $ 10 $ です。