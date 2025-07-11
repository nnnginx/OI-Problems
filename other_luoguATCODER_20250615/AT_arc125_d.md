# AT_arc125_d [ARC125D] Unique Subsequence

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc125/tasks/arc125_d

長さ $ N $ の整数列 $ A_1,A_2,\cdots,A_N $ が与えられます．

$ A $ の非空な部分列 $ s $ であって，以下の条件を満たすものの個数を $ 998244353 $ で割った余りを求めてください．

- $ A $ から $ s $ を取り出す方法が一意である． つまり，$ s=(s_1,s_2,\cdots,s_k) $ とした時，$ A_{idx(i)}=s_i $ ($ 1\ \leq\ i\ \leq\ k $)を満たす添字の列 $ 1\ \leq\ idx(1)\ <\ idx(2)\ <\ \cdots\ <\ idx(k)\ \leq\ N $ がちょうど一つ存在する．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ N $ $ A_1 $ $ A_2 $ $ \cdots $ $ A_N $

## 输出格式

答えを出力せよ．

## 输入输出样例 #1

### 输入 #1

```
3
1 2 1
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
4
4 2 1 3
```

### 输出 #2

```
15
```

## 输入输出样例 #3

### 输入 #3

```
12
1 2 3 6 9 2 3 3 9 6 1 6
```

### 输出 #3

```
1178
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ N $
- 入力される値はすべて整数である

### Sample Explanation 1

以下の $ 5 $ つの部分列が条件を満たします． - $ (1,1) $ - $ (1,2) $ - $ (1,2,1) $ - $ (2) $ - $ (2,1) $ 部分列 $ (1) $ は取り出す方法が $ 2 $ 通りあるので条件を満たしません．