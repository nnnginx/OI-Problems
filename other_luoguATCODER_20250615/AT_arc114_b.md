# AT_arc114_b [ARC114B] Special Subsets

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc114/tasks/arc114_b

$ 1 $ 以上 $ N $ 以下の整数すべてから成る集合を $ S $ とします．

$ f $ は $ S $ から $ S $ への関数であり，$ f(1),\ f(2),\ \cdots,\ f(N) $ の値が $ f_1,\ f_2,\ \cdots,\ f_N $ として与えられます．

$ S $ の空でない部分集合 $ T $ であって，次の両方の条件を満たすものの個数を $ 998244353 $ で割った余りを求めてください．

- 全ての $ a\ \in\ T $ について $ f(a)\ \in\ T $ である．
- 全ての $ a,\ b\ \in\ T $ について $ a\ \neq\ b $ ならば $ f(a)\ \neq\ f(b) $ である．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ N $ $ f_1 $ $ f_2 $ $ \ldots $ $ f_N $

## 输出格式

$ S $ の空でない部分集合であって，両方の条件を満たすものの個数を $ 998244353 $ で割った余りを出力せよ．

## 输入输出样例 #1

### 输入 #1

```
2
2 1
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
2
1 1
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
3
1 2 3
```

### 输出 #3

```
7
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ f_i\ \leq\ N $
- 入力は全て整数

### Sample Explanation 1

$ f(1)\ =\ 2,\ f(2)\ =\ 1 $ です．$ f(1)\ \neq\ f(2) $ であるため条件の $ 2 $ つ目は常に満たしますが，$ 1 $ つ目の条件より $ 1,\ 2 $ は同時に $ T $ に入っている必要があります．

### Sample Explanation 2

$ f(1)\ =\ f(2)\ =\ 1 $ です．$ 1 $ つ目の条件のため $ 1 $ は $ T $ に属する必要があり，さらに $ 2 $ つ目の条件により $ 2 $ は $ T $ に属することはできません．

### Sample Explanation 3

$ f(1)\ =\ 1,\ f(2)\ =\ 2,\ f(3)\ =\ 3 $ です．$ 1 $ つ目の条件も $ 2 $ つ目の条件も常に満たされるため，$ S $ の空でない部分集合全てが条件を満たします．