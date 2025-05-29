## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc247/tasks/abc247_e

長さ $ N $ の数列 $ A\ =\ (A_1,\ A_2,\ \dots,\ A_N) $ および整数 $ X,\ Y $ があります。 次の条件をすべて満たす整数の組 $ (L,\ R) $ の個数を求めてください。

- $ 1\ \leq\ L\ \leq\ R\ \leq\ N $
- $ A_L,\ A_{L+1},\ \dots,\ A_R $ の最大値は $ X $ であり、最小値は $ Y $ である。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ X $ $ Y $ $ A_1 $ $ A_2 $ $ \dots $ $ A_N $

## 输出格式
答えを出力せよ。

## 题目大意
给定数列 $ A_n $，给定 $ X, Y $，我们定义数对 $ (L, R) $ 满足 $ 1 \le L \le R \le n $，且数列 $ A_L, A_{L + 1}, \cdots, A_R $ 满足最大值为 $ X $，最小值为 $ Y $，求有多少种满足条件的数对。

```input1
4 3 1
1 2 3 1
```

```output1
4
```

```input2
5 2 1
1 3 2 4 1
```

```output2
0
```

```input3
5 1 1
1 1 1 1 1
```

```output3
15
```

```input4
10 8 1
2 7 1 8 2 8 1 8 2 8
```

```output4
36
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ Y\ \leq\ X\ \leq\ 2\ \times\ 10^5 $
- 入力される値はすべて整数である。

### Sample Explanation 1

条件を満たすのは $ (L,R)=(1,3),(1,4),(2,4),(3,4) $ の $ 4 $ 通りです。

### Sample Explanation 2

条件を満たす $ (L,R) $ は存在しません。

### Sample Explanation 3

$ X=Y $ である場合もあります。

