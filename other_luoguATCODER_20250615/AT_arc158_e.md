# AT_arc158_e [ARC158E] All Pair Shortest Paths

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc158/tasks/arc158_e

$ 2 $ 行 $ N $ 列のマス目があります．上から $ i $ 行目，左から $ j $ 列目のマスを $ (i,j) $ で表します．$ (i,j) $ には正整数 $ x_{i,j} $ が書かれています．

$ 2 $ つのマスは，辺を共有するときに**隣接する**といいます．

マス $ X $ から $ Y $ への**パス**とは，相異なるマスからなる列 $ (P_1,\ \ldots,\ P_n) $ であって，$ P_1\ =\ X $, $ P_n\ =\ Y $ であり，任意の $ 1\leq\ i\ \leq\ n-1 $ に対して $ P_i $ と $ P_{i+1} $ が隣接するものをいいます．さらに，そのパスの**重み**を $ P_1,\ \ldots,\ P_n $ に書かれている整数の総和として定義します．

$ 2 $ つのマス $ X,\ Y $ に対して，$ X $ から $ Y $ へのパスの重みとしてありうる最小値を $ f(X,\ Y) $ と書くことにします．すべてのマスの $ 2 $ つ組 $ (X,Y) $ に対する $ f(X,\ Y) $ の総和を $ 998244353 $ で割った余りを求めてください．

## 输入格式

入力は以下の形式で標準入力から与えられます．

> $ N $ $ x_{1,1} $ $ \ldots $ $ x_{1,N} $ $ x_{2,1} $ $ \ldots $ $ x_{2,N} $

## 输出格式

すべてのマスの $ 2 $ つ組 $ (X,Y) $ に対する $ f(X,\ Y) $ の総和を $ 998244353 $ で割った余りを出力してください．

## 输入输出样例 #1

### 输入 #1

```
1
3
5
```

### 输出 #1

```
24
```

## 输入输出样例 #2

### 输入 #2

```
2
1 2
3 4
```

### 输出 #2

```
76
```

## 输入输出样例 #3

### 输入 #3

```
5
1 1000000000 1 1 1
1 1 1 1000000000 1
```

### 输出 #3

```
66714886
```

## 说明/提示

### 制約

- $ 1\leq\ N\leq\ 2\times\ 10^5 $
- $ 1\leq\ x_{i,j}\ \leq\ 10^9 $
 
### Sample Explanation 1

次の $ 4 $ 通りの値の総和を求めます． - $ X\ =\ (1,1),\ Y\ =\ (1,1) $ のとき：$ f(X,\ Y)\ =\ 3 $． - $ X\ =\ (1,1),\ Y\ =\ (2,1) $ のとき：$ f(X,\ Y)\ =\ 8 $． - $ X\ =\ (2,1),\ Y\ =\ (1,1) $ のとき：$ f(X,\ Y)\ =\ 8 $． - $ X\ =\ (2,1),\ Y\ =\ (2,1) $ のとき：$ f(X,\ Y)\ =\ 5 $．