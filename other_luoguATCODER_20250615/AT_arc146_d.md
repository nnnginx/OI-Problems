# AT_arc146_d [ARC146D] >=<

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc146/tasks/arc146_d

長さ $ N $ かつ全要素が $ 1 $ 以上 $ M $ 以下の整数列 $ A=(A_1,A_2,\dots,A_N) $ であって、以下の条件を全て満たすものを「素晴らしい整数列」と呼びます。

- $ 1\ \le\ i\ \le\ K $ を満たす整数 $ i $ に対して、以下のうちのいずれかが成り立つ。
  - $ A_{P_i}\ <\ X_i $ かつ $ A_{Q_i}\ <\ Y_i $
  - $ A_{P_i}\ =\ X_i $ かつ $ A_{Q_i}\ =\ Y_i $
  - $ A_{P_i}\ >\ X_i $ かつ $ A_{Q_i}\ >\ Y_i $

「素晴らしい整数列」が存在するか判定し、存在するならば「素晴らしい整数列」の要素の総和としてあり得る最小値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ K $ $ P_1 $ $ X_1 $ $ Q_1 $ $ Y_1 $ $ P_2 $ $ X_2 $ $ Q_2 $ $ Y_2 $ $ \vdots $ $ P_K $ $ X_K $ $ Q_K $ $ Y_K $

## 输出格式

「素晴らしい整数列」が存在する場合は「素晴らしい整数列」の要素の総和としてあり得る最小値を、「素晴らしい整数列」が存在しない場合は $ -1 $ を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 4 3
3 1 1 2
1 1 2 2
3 4 1 4
```

### 输出 #1

```
6
```

## 输入输出样例 #2

### 输入 #2

```
2 2 2
1 1 2 2
2 1 1 2
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
5 10 10
4 1 2 7
5 1 3 2
2 9 4 4
5 4 2 9
2 9 1 9
4 8 3 10
5 7 1 5
3 5 1 2
3 8 2 10
2 9 4 8
```

### 输出 #3

```
12
```

## 说明/提示

### 制約

- $ 1\ \le\ N,M,K\ \le\ 2\ \times\ 10^5 $
- $ 1\ \le\ P_i,Q_i\ \le\ N $
- $ 1\ \le\ X_i,Y_i\ \le\ M $
- $ P_i\ \neq\ Q_i $
- 入力は全て整数である。

### Sample Explanation 1

$ A=(2,3,1) $ は全ての条件を満たすので「素晴らしい整数列」です。この場合要素の総和は $ 6 $ です。 要素の総和が $ 5 $ 以下の「素晴らしい整数列」は存在しないため、解は $ 6 $ です。

### Sample Explanation 2

「素晴らしい整数列」は存在しないため、$ -1 $ を出力します。