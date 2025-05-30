## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc145/tasks/arc145_a

`A`, `B` からなる長さ $ N $ の文字列 $ S $ が与えられます。

あなたは、以下の操作を $ 0 $ 回以上好きな回数繰り返すことができます。

- $ S $ の中の隣接する $ 2 $ 文字を一ヶ所選び、`AB` で置き換える。

$ S $ を回文にできるか判定してください。

 回文とは ある文字列 $ T $ について、 $ T $ の長さを $ |T| $ として、全ての整数 $ i $ ($ 1\ \le\ i\ \le\ |T| $) について、 $ T $ の前から $ i $ 文字目と後ろから $ i $ 文字目が同じであるとき、またそのときに限って、 $ T $ は回文です。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式
$ S $ を回文にできる場合は `Yes` を、そうでない場合は `No` を出力せよ。

## 题目大意
给定长为 $n$
，由 $A$ 和 $B$ 组成的字符串，每次可以选择相邻两位替换成 $AB$。
询问原字符串是否能通过若干次操作变成回文字符串。

```input1
3
BBA
```

```output1
Yes
```

```input2
4
ABAB
```

```output2
No
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ S $ は `A`, `B` からなる長さ $ N $ の文字列

### Sample Explanation 1

$ 2,3 $ 文字目の `BA` を操作により `AB` で置き換えることで、$ S $ を回文である `BAB` にできます。

### Sample Explanation 2

操作を何回行っても、$ S $ を回文にはできません。

