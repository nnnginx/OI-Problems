## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc123/tasks/arc123_d

整数列 $ A\ =\ (A_1,\ \ldots,\ A_N) $ が与えられます。

整数列 $ B\ =\ (B_1,\ \ldots,\ B_N) $ および $ C\ =\ (C_1,\ \ldots,\ C_N) $ の組であって、以下の条件を満たすものを考えます：

- $ 1\leq\ i\leq\ N $ に対して $ A_i\ =\ B_i\ +\ C_i $ が成り立つ。
- $ B $ は広義単調増加である。つまり $ 1\leq\ i\leq\ N-1 $ に対して $ B_i\leq\ B_{i+1} $ が成り立つ。
- $ C $ は広義単調減少である。つまり $ 1\leq\ i\leq\ N-1 $ に対して $ C_i\geq\ C_{i+1} $ が成り立つ。

$ \sum_{i=1}^N\ \bigl(\lvert\ B_i\rvert\ +\ \lvert\ C_i\rvert\bigr) $ としてありうる最小値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられます。

> $ N $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式
答えを出力してください。

## 题目大意
给出长为 $n$ 的序列 $a$，构造长为 $n$ 的序列 $b,c$，要求：

- $b$ 非严格递增。
- $c$ 非严格递减。
- $b_i+c_i=a_i$ 。

最小化 $\sum_{i=1}^n |b_i|+|c_i|$。

```input1
3
1 -2 3
```

```output1
10
```

```input2
4
5 4 3 5
```

```output2
17
```

```input3
1
-10
```

```output3
10
```

## 提示
### 制約

- $ 1\leq\ N\leq\ 2\times\ 10^5 $
- $ -10^8\leq\ A_i\leq\ 10^8 $

### Sample Explanation 1

最小値を与える整数列 $ B $, $ C $ として、例えば次があります： - $ B\ =\ (0,\ 0,\ 5) $ - $ C\ =\ (1,\ -2,\ -2) $ $ \sum_{i=1}^N\ \bigl(\lvert\ B_i\rvert\ +\ \lvert\ C_i\rvert\bigr)\ =\ (0+1)\ +\ (0+2)\ +\ (5+2)\ =\ 10 $ となっています。

### Sample Explanation 2

最小値を与える整数列 $ B $, $ C $ として、例えば次があります： - $ B\ =\ (0,\ 1,\ 2,\ 4) $ - $ C\ =\ (5,\ 3,\ 1,\ 1) $

### Sample Explanation 3

最小値を与える整数列 $ B $, $ C $ として、例えば次があります： - $ B\ =\ (-3) $ - $ C\ =\ (-7) $

