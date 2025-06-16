## 题目描述
[problemUrl]: https://atcoder.jp/contests/toyota2023spring-final/tasks/toyota2023spring_final_f

`A`, `B` からなる長さ $ N $ の文字列 $ S $ が与えられます．

あなたは，以下の操作を $ 0 $ 回以上繰り返すことができます．

- $ S $ 中の連続する $ 2 $ 文字であって，`AB` で**ない**ものを選び，消す． その後，残った左右の（空かもしれない）文字列を連結し，これを新たに $ S $ とする．

操作後の $ S $ としてあり得る文字列が何通りあるかを $ 998244353 $ で割ったあまりを求めてください．

## 输入格式
入力は以下の形式で標準入力から与えられる．

> $ N $ $ S $

## 输出格式
答えを出力せよ．

## 题目大意
给你一个长度为 $n$、由 `A` 和 `B` 组成的字符串 $S$，每次操作你可以删除连续的不是 `AB` 的两个字符。求经过任意次操作（包括 $0$ 次）后本质不同的剩余字符串数。对 $998244353$ 取模。

```input1
3
BBA
```

```output1
3
```

```input2
5
ABABA
```

```output2
3
```

```input3
9
BABBAAAAB
```

```output3
14
```

```input4
48
AABABBBAABAAABAAABBBAAABBBAABAABBABAABBAAAAABBBB
```

```output4
3073910
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 10^6 $
- $ S $ は `A`, `B` からなる長さ $ N $ の文字列である

### Sample Explanation 1

操作後の $ S $ としてありうる文字列は，`A`, `B`, `BBA` の $ 3 $ 通りです．

### Sample Explanation 2

操作後の $ S $ としてありうる文字列は，`A`, `ABA`, `ABABA` の $ 3 $ 通りです．

