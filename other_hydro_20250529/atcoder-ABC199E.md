## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc199/tasks/abc199_e

$ (1,\ 2,\ 3,\ \dots,\ N) $ を並び替えてできる数列 $ a $ であって、以下の条件を満たすものの数を出力してください。

- $ 1\ \le\ i\ \le\ M $ を満たす全ての整数 $ i $ について、$ a_1,\ a_2,\ a_3,\ \dots,\ a_{X_i} $ の中に $ Y_i $ 以下の数は $ Z_i $ 個以下しか存在しない

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ X_1 $ $ Y_1 $ $ Z_1 $ $ X_2 $ $ Y_2 $ $ Z_2 $ $ X_3 $ $ Y_3 $ $ Z_3 $ $ \hspace{23pt}\ \vdots $ $ X_M $ $ Y_M $ $ Z_M $

## 输出格式
答えを出力せよ。

## 题目大意
第一行给定 $n$ 和 $m$。后 $m$ 行，每行给定一个规则。

- 规则：后 $m$ 行每行给出三个整数 $X_i,Y_i,Z_i$，表示在排列的前 $X_i$ 个数字中最多只能有 $Z_i$ 个数字小于等于 $Y_i$。

构造长度为 $n$ 的排列，求最多可以构造多少个满足所有规则的排列。

```input1
3 1
2 2 1
```

```output1
4
```

```input2
5 2
3 3 2
4 4 3
```

```output2
90
```

```input3
18 0
```

```output3
6402373705728000
```

## 提示
### 制約

- $ 2\ \le\ N\ \le\ 18 $
- $ 0\ \le\ M\ \le\ 100 $
- $ 1\ \le\ X_i\ \lt\ N $
- $ 1\ \le\ Y_i\ \lt\ N $
- $ 0\ \le\ Z_i\ \lt\ N $
- 入力に含まれる値は全て整数である

### Sample Explanation 1

条件を満たす $ a $ は以下の $ 4 $ つです。 - $ (1,\ 3,\ 2) $ - $ (2,\ 3,\ 1) $ - $ (3,\ 1,\ 2) $ - $ (3,\ 2,\ 1) $ $ (1,\ 2,\ 3) $ や $ (2,\ 1,\ 3) $ は、$ a_1,\ a_2 $ の中に $ 2 $ 以下の数が $ 2 $ つあるため条件を満たしません。

