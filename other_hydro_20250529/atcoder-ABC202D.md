## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc202/tasks/abc202_d

$ A $ 個の `a` と $ B $ 個の `b` からなる長さ $ A\ +\ B $ の文字列のうち、辞書順で $ K $ 番目のものを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ K $

## 输出格式
答えを出力せよ。

## 题目大意
### 【题意简述】
给定 $A,B,K$ 三个正整数。

求以 $A$ 个 $a$ ， $B$ 个 $b$ 组成的长度为 $A\ +\ B$ 字符串的若干种可能中，按词典序的第 $K$ 种可能。
### 【数据范围】
令 $S$ 所有的可能数目。

$ 1 ≤ A, B ≤ 30 $

$1 ≤ K ≤ S$

```input1
2 2 4
```

```output1
baab
```

```input2
30 30 118264581564861424
```

```output2
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
```

## 提示
### 制約

- $ 1\ \leq\ A,\ B\ \leq\ 30 $
- $ A $ 個の `a` と $ B $ 個の `b` からなる長さ $ A\ +\ B $ の文字列の総数を $ S $ 個とおいたとき、$ 1\ \leq\ K\ \leq\ S $
- 入力は全て整数である。

### Sample Explanation 1

$ 2 $ 個の `a` と $ 2 $ 個の `b` からなる文字列を辞書順に並べると、`aabb`、`abab`、`abba`、`baab`、`baba`、`bbaa` となります。 よって、$ 4 $ 番目である `baab` を出力します。

### Sample Explanation 2

$ K $ の値は $ 32 $ bit 整数に収まらないことがあります。

