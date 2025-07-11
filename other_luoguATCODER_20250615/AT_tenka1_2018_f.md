# AT_tenka1_2018_f Circular

## 题目描述

[problemUrl]: https://atcoder.jp/contests/tenka1-2018/tasks/tenka1_2018_f

整数 $ N $ 個からなる列 $ A_1,A_2,...,A_N $ が与えられます。

$ 1,2,...,N $ の並び替え $ p_1,p_2,...,p_N $ であって、 次の操作を何度か行うことでこの列を $ A_1,A_2,...,A_N $ に変換できるようなものの個数を $ 998244353 $ で割ったあまりを求めてください。

- 各 $ 1\leq\ i\leq\ N $ に対し、$ q_i=min(p_{i-1},p_{i}) $ とする。ただし、$ p_0=p_N $ とする。列 $ p $ を列 $ q $ で置き換える。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ : $ $ A_N $

## 输出格式

条件を満たす列の個数を $ 998244353 $ で割ったあまりを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
1
2
1
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
5
3
1
4
1
5
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
8
4
4
4
1
1
1
2
2
```

### 输出 #3

```
24
```

## 输入输出样例 #4

### 输入 #4

```
6
1
1
6
2
2
2
```

### 输出 #4

```
0
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 3\ ×\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ N $
- 入力はすべて整数である

### Sample Explanation 1

$ (2,3,1),(3,2,1) $ が条件を満たします。