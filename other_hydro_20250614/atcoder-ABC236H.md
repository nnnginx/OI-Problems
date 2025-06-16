## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc236/tasks/abc236_h

正整数 $ N,\ M $ および正整数列 $ D\ =\ (D_1,\ \dots,\ D_N) $ が与えられます。

以下の条件を満たす正整数列 $ A\ =\ (A_1,\ \dots,\ A_N) $ の総数を $ 998244353 $ で割った余りを求めてください。

- $ 1\ \leq\ A_i\ \leq\ M\ \,\ (1\ \leq\ i\ \leq\ N) $
- $ A_i\ \neq\ A_j\ \,\ (1\ \leq\ i\ \lt\ j\ \leq\ N) $
- 各 $ i\ \,\ (1\ \leq\ i\ \leq\ N) $ について、$ A_i $ は $ D_i $ の倍数

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ D_1 $ $ \ldots $ $ D_N $

## 输出格式
答えを出力せよ。

## 题目大意
给定两个正整数 $N,M$ 和一个正整数序列 $D$，询问满足条件的序列 $A$ 的个数：

1. $1\leq A_i\leq M(1\leq i\leq N)$
2. $A_i\neq A_j(1\leq i<j\leq N)$
3. $D_i|A_i$

- $2\leq N\leq 16,1\leq M\leq 10^{18},1\leq D_i\leq M$

```input1
3 7
2 3 4
```

```output1
3
```

```input2
3 3
1 2 2
```

```output2
0
```

```input3
6 1000000000000000000
380214083 420492929 929717250 666796775 209977152 770361643
```

```output3
325683519
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 16 $
- $ 1\ \leq\ M\ \leq\ 10^{18} $
- $ 1\ \leq\ D_i\ \leq\ M\ \,\ (1\ \leq\ i\ \leq\ N) $
- 入力は全て整数である。

### Sample Explanation 1

条件を満たす $ A $ は $ (2,\ 3,\ 4),\ (2,\ 6,\ 4),\ (6,\ 3,\ 4) $ の $ 3 $ 通りです。

### Sample Explanation 2

条件を満たす $ A $ は存在しません。

### Sample Explanation 3

$ 998244353 $ で割った余りを求めることに注意してください。

