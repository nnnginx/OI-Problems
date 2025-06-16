# AT_arc166_d [ARC166D] Interval Counts

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc166/tasks/arc166_d

$ x_1\ <\ \cdots\ <\ x_N $ を満たす正整数 $ x_1,\ \ldots,\ x_N $ および，正整数 $ y_1,\ \ldots,\ y_N $ が与えられます．

組 $ (M,\ L_1,\ R_1,\ \ldots,\ L_M,\ R_M) $ であって，以下の条件を全て満たすものを考えます：

- $ M $ は正整数である．
- 各 $ j\ (1\leq\ j\leq\ M) $ に対して，$ L_j,\ R_j $ は $ L_j\leq\ R_j $ を満たす整数である．
- 各 $ i\ (1\leq\ i\leq\ N) $ に対して，$ L_j\leq\ x_i\leq\ R_j $ を満たす $ j\ (1\leq\ j\leq\ M) $ がちょうど $ y_i $ 個存在する．
 
このような組は必ず存在することが証明できます．そのような組に対する $ \min\ \lbrace\ R_j-L_j\mid\ 1\leq\ j\leq\ M\rbrace $ としてありうる最大値を求めてください．ただし，最大値が存在しない場合には `-1` を出力してください．

## 输入格式

入力は以下の形式で標準入力から与えられます．

> $ N $ $ x_1 $ $ \cdots $ $ x_N $ $ y_1 $ $ \cdots $ $ y_N $

## 输出格式

条件を満たす組に対する $ \min\ \lbrace\ R_j-L_j\mid\ 1\leq\ j\leq\ M\rbrace $ としてありうる最大値を出力してください．ただし，最大値が存在しない場合には `-1` を出力してください．

## 输入输出样例 #1

### 输入 #1

```
3
1 3 5
1 3 1
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
3
1 10 100
2 3 2
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
7
10 31 47 55 68 73 90
3 7 4 6 3 4 4
```

### 输出 #3

```
56
```

## 说明/提示

### 制約

- $ 1\leq\ N\leq\ 2\times\ 10^5 $
- $ 1\leq\ x_1\ <\ \cdots\ <\ x_N\ \leq\ 10^9 $
- $ 1\leq\ y_i\ \leq\ 10^9 $
 
### Sample Explanation 1

例えば組 $ (3,\ 1,\ 4,\ 2,\ 4,\ 3,\ 5) $ に対して $ \min\ \lbrace\ R_j-L_j\mid\ 1\leq\ j\leq\ M\rbrace\ =\ 2 $ が成り立ちます．

### Sample Explanation 2

例えば組 $ (3,\ -1000,\ 10,\ -1000,\ 1000,\ 10,\ 1000) $ に対して $ \min\ \lbrace\ R_j-L_j\mid\ 1\leq\ j\leq\ M\rbrace\ =\ 990 $ が成り立ちます．$ \min\ \lbrace\ R_j-L_j\mid\ 1\leq\ j\leq\ M\rbrace $ の最大値は存在しません．