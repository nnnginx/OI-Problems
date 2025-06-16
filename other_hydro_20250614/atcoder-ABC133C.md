## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc133/tasks/abc133_c

非負整数 $ L,\ R $ が与えられます。 $ 2 $ つの整数 $ i,\ j $ を $ L\ \leq\ i\ <\ j\ \leq\ R $ を満たすように選びます。 $ (i\ \times\ j)\ \text{\ mod\ }\ 2019 $ の最小値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ L $ $ R $

## 输出格式
条件を満たすように $ i,\ j $ を選んだ時の、$ (i\ \times\ j)\ \text{\ mod\ }\ 2019 $ の最小値を出力せよ。

## 题目大意
### 题目描述
给出非负整数 $L$ 和 $R$，在这个区间里选择两个整数 $i$ 和 $j$ 满足 $L\le i < j\le R$。求 $(i\times j)\mod 2019$ 的最小值。
### 输入格式
$L$ 和 $R$
### 输出格式
$(i\times j)\mod 2019$ 的最小值
### 数据范围
$ 0 \le L < R \le 2 \times 10^9$

```input1
2020 2040
```

```output1
2
```

```input2
4 5
```

```output2
20
```

## 提示
### 制約

- 入力は全て整数
- $ 0\ \leq\ L\ <\ R\ \leq\ 2\ \times\ 10^9 $

### Sample Explanation 1

$ (i,\ j)\ =\ (2020,\ 2021) $ とすると、$ (i\ \times\ j)\ \text{\ mod\ }\ 2019\ =\ 2 $ となります。

### Sample Explanation 2

選び方は $ (i,\ j)\ =\ (4,\ 5) $ の $ 1 $ 通りしか存在しません。

