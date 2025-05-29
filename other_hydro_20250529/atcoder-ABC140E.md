## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc140/tasks/abc140_e

$ \{1,\ 2,\ \ldots,\ N\} $ の順列 $ P $ が与えられます。

ペア $ (L,\ R)\ (1\ \le\ L\ \lt\ R\ \le\ N) $について、$ P_L,\ P_{L+1},\ \ldots,\ P_R $ の中で $ 2 $ 番目に大きいものを $ X_{L,\ R} $ とします。

$ \displaystyle\ \sum_{L=1}^{N-1}\ \sum_{R=L+1}^{N}\ X_{L,R} $ を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ P_1 $ $ P_2 $ $ \ldots $ $ P_N $

## 输出格式
$ \displaystyle\ \sum_{L=1}^{N-1}\ \sum_{R=L+1}^{N}\ X_{L,R} $ を出力せよ。

## 题目大意
给定一个N的排列P，对于区间[l, r]，其中l < r，求所有区间[l, r]中第二大的数的和。

```input1
3
2 3 1
```

```output1
5
```

```input2
5
1 2 3 4 5
```

```output2
30
```

```input3
8
8 2 7 3 4 5 6 1
```

```output3
136
```

## 提示
### 制約

- $ 2\ \le\ N\ \le\ 10^5 $
- $ 1\ \le\ P_i\ \le\ N $
- $ P_i\ \neq\ P_j $ $ (i\ \neq\ j) $
- 入力はすべて整数

### Sample Explanation 1

$ X_{1,\ 2}\ =\ 2,\ X_{1,\ 3}\ =\ 2,\ X_{2,\ 3}\ =\ 1 $ より、総和は $ 2\ +\ 2\ +\ 1\ =\ 5 $ となります。

