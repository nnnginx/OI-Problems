## 题目描述
[problemUrl]: https://atcoder.jp/contests/code-festival-2017-quala/tasks/code_festival_2017_quala_a

りんごさんは、すぬけ君にプレゼントを贈ろうとしています。

すぬけ君の好物が焼肉であることを知ったりんごさんは、すぬけ君は名前が `YAKI` から始まるものを好み、そうでないものを好まないと判断しました。

りんごさんが贈ろうと思っているものの名前を表す文字列 $ S $ が与えられます。$ S $ が `YAKI` から始まるかどうか判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
$ S $ が `YAKI` から始まるなら `Yes` を、そうでないなら `No` を出力せよ。

## 题目大意
输入一个字符串，判断是否以“YAKI”开头，如果是，输出“Yes”，否则输出“No”。
长度范围：
1≤S的绝对值≤10

```input1
YAKINIKU
```

```output1
Yes
```

```input2
TAKOYAKI
```

```output2
No
```

```input3
YAK
```

```output3
No
```

## 提示
### 制約

- $ 1\ \leq\ |S|\ \leq\ 10 $
- $ S $ は英大文字からなる

### Sample Explanation 1

`YAKINIKU` は `YAKI` で始まります。

### Sample Explanation 2

`TAKOYAKI` は `YAKI` で始まりません。

