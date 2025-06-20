# AT_jsc2019_final_d Minimize Maximum

## 题目描述

[problemUrl]: https://atcoder.jp/contests/jsc2019-final/tasks/jsc2019_final_d

長さ $ N $ の整数列 $ A_0,A_1,\cdots,A_{N-1} $ と $ B_0,B_1,\cdots,B_{N-1} $ が与えられます。

全ての $ k $ ($ 2\ \leq\ k\ \leq\ N $) について、次の問題を解いてください。

- 整数列 $ C_0,C_1,\cdots,C_{k-1} $ をつくる。 ここで、全ての $ i $ ($ 0\ \leq\ i\ \leq\ k-1 $) について、$ A_i\ \leq\ C_i\ \leq\ B_i $ を満たさなくてはならない。 「$ C_{i+1}-C_i $ ($ 0\ \leq\ i\ \leq\ k-2 $) の最大値」としてありうる最小の値はいくらか。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_0 $ $ A_1 $ $ \cdots $ $ A_{N-1} $ $ B_0 $ $ B_1 $ $ \cdots $ $ B_{N-1} $

## 输出格式

$ N-1 $ 行出力せよ。$ i $ ($ 1\ \leq\ i\ \leq\ N-1 $) 行目には、$ k=i+1 $ のときの問題の答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4
0 0 1 2
2 1 3 3
```

### 输出 #1

```
-2
0
1
```

## 输入输出样例 #2

### 输入 #2

```
10
24 8 6 8 13 25 4 1 4 7
100 89 65 46 66 58 22 16 11 10
```

### 输出 #2

```
-92
-47
-30
-21
-10
-10
-10
-8
-4
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 0\ \leq\ A_i\ \leq\ B_i\ \leq\ 10^9 $
- 入力される値はすべて整数である。

### Sample Explanation 1

各 $ k $ について、「$ C_{i+1}-C_i $ の最大値」が最小になる整数列 $ C $ の例を示します。 - $ k=2 $: $ C=(2,0) $ - $ k=3 $: $ C=(1,1,1) $ - $ k=4 $: $ C=(1,1,1,2) $