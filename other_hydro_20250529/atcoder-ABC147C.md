## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc147/tasks/abc147_c

$ 1 $ から $ N $ までの番号がついた $ N $ 人の人がいます。彼らはみな、必ず正しい証言を行う「正直者」か、真偽不明の証言を行う「不親切な人」のいずれかです。

人 $ i $ は $ A_i $ 個の証言を行っています。人 $ i $ の $ j $ 個目の証言は $ 2 $ つの整数 $ x_{ij} $ , $ y_{ij} $ で表され、$ y_{ij}\ =\ 1 $ のときは「人 $ x_{ij} $ は正直者である」という証言であり、$ y_{ij}\ =\ 0 $ のときは「人 $ x_{ij} $ は不親切な人である」という証言です。

この $ N $ 人の中には最大で何人の正直者が存在し得るでしょうか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ x_{11} $ $ y_{11} $ $ x_{12} $ $ y_{12} $ $ : $ $ x_{1A_1} $ $ y_{1A_1} $ $ A_2 $ $ x_{21} $ $ y_{21} $ $ x_{22} $ $ y_{22} $ $ : $ $ x_{2A_2} $ $ y_{2A_2} $ $ : $ $ A_N $ $ x_{N1} $ $ y_{N1} $ $ x_{N2} $ $ y_{N2} $ $ : $ $ x_{NA_N} $ $ y_{NA_N} $

## 输出格式
存在し得る正直者の最大人数を出力せよ。

## 题目大意
​	现在有 $N$ 个人的编号为 $1$ 到 $N$ .

​	 对于其中任意一个人而言，如果他是诚实的，则他的证言总是正确的；否则他就是虚伪的，他的证言可能正确，也可能错误。

​	现在，第 $i$ 个人有 $A_i$ 条证言。对于他的第 $j$ 条证言由两个数组成：$x_{i,j}$，$y_{i,j}$.

​	则此证言表示的含义为：如果 $y_{i,j} = 1$，则此人认为编号为 $x_{i,j}$ 的人是诚实的；如果 $y_{i,j} = 0$，则此人认为编号为 $x_{i,j}$ 的人是虚伪的。

​	那么，请输出可能存在的最多的诚实的人的数量。

```input1
3
1
2 1
1
1 1
1
2 0
```

```output1
2
```

```input2
3
2
2 1
3 0
2
3 1
1 0
2
1 1
2 0
```

```output2
0
```

```input3
2
1
2 0
1
1 0
```

```output3
1
```

## 提示
### 制約

- 入力は全て整数
- $ 1\ <\ =\ N\ <\ =\ 15 $
- $ 0\ \leq\ A_i\ \leq\ N\ -\ 1 $
- $ 1\ \leq\ x_{ij}\ \leq\ N $
- $ x_{ij}\ \neq\ i $
- $ x_{ij_1}\ \neq\ x_{ij_2}\ (j_1\ \neq\ j_2) $
- $ y_{ij}\ =\ 0,\ 1 $

### Sample Explanation 1

人 $ 1 $ と人 $ 2 $ が正直者であり、人 $ 3 $ が不親切な人であると仮定すると、正直者は $ 2 $ 人であり、矛盾が生じません。これが存在し得る正直者の最大人数です。

### Sample Explanation 2

$ 1 $ 人でも正直者が存在すると仮定すると、直ちに矛盾します。

