# AT_agc022_c [AGC022C] Remainder Game

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc022/tasks/agc022_c

アオキは数列 $ a_{1},\ a_{2},\ ...,\ a_{N} $ で遊んでいます。$ 1 $ 秒ごとに、アオキは次の操作を行います。

- 正の整数 $ k $ を選ぶ。数列のそれぞれの要素 $ v $ について、アオキは $ v $ を「$ v $ を $ k $ で割った余り」に置き換えるか、$ v $ をそのままにするかを選べる。この一連の操作のコストは（書き換えた要素の数によらず）$ 2^{k} $ である。

アオキは、数列を $ b_{1},\ b_{2},\ ...,\ b_{N} $ に変えたいです（要素の順番も考慮します）。この目的を達成することが可能か判定し、可能である場合は必要な最小のコストを求めてください。

## 输入格式

入力は標準入力から以下の形式で与えられる。

> $ N $ $ a_{1} $ $ a_{2} $ $ ... $ $ a_{N} $ $ b_{1} $ $ b_{2} $ $ ... $ $ b_{N} $

## 输出格式

はじめの数列を $ b_{1},\ b_{2},\ ...,\ b_{N} $ に変えるのに必要な最小のコストを出力せよ。目的の達成が不可能である場合は、代わりに $ -1 $ と出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
19 10 14
0 3 4
```

### 输出 #1

```
160
```

## 输入输出样例 #2

### 输入 #2

```
3
19 15 14
0 0 0
```

### 输出 #2

```
2
```

## 输入输出样例 #3

### 输入 #3

```
2
8 13
5 13
```

### 输出 #3

```
-1
```

## 输入输出样例 #4

### 输入 #4

```
4
2 0 1 8
2 0 1 8
```

### 输出 #4

```
0
```

## 输入输出样例 #5

### 输入 #5

```
1
50
13
```

### 输出 #5

```
137438953472
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 50 $
- $ 0\ \leq\ a_{i},\ b_{i}\ \leq\ 50 $
- 入力中の値はすべて整数である。

### Sample Explanation 1

操作手順の例を挙げます。 - $ k\ =\ 7 $ を選ぶ。$ 19 $ を $ 5 $ に、$ 10 $ を $ 3 $ に置き換えて $ 14 $ はそのままにする。数列は $ 5,\ 3,\ 14 $ となる。 - $ k\ =\ 5 $ を選ぶ。$ 5 $ を $ 0 $ に置き換え、$ 3 $ はそのままにして $ 14 $ を $ 4 $ に置き換える。数列は $ 0,\ 3,\ 4 $ となる。 合計コストは $ 2^{7}\ +\ 2^{5}\ =\ 160 $ です。

### Sample Explanation 2

$ k\ =\ 1 $ を選び、すべてを $ 0 $ に変えるとよいです。コストは $ 2^{1}\ =\ 2 $ です。

### Sample Explanation 3

与えられた操作では $ 8 $ を $ 5 $ に変えることができないため、目的の達成は不可能です。

### Sample Explanation 4

この場合は何もする必要がありません。コストは $ 0 $ です。

### Sample Explanation 5

オーバーフローにご注意。