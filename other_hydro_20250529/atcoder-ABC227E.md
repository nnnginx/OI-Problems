## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc227/tasks/abc227_e

`K`, `E`, `Y` のみからなる文字列 $ S $ が与えられます。

$ S $ の隣接する $ 2 $ 文字を入れ替える操作を $ K $ 回まで行えるとき、作ることができる文字列は何種類ありますか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $ $ K $

## 输出格式
答えを出力せよ。

## 题目大意
给定一个字符串 $S$ 和一个非负整数 $K$，求从 $S$ 开始至多进行 $K$ 次相邻字符的交换，可以生成多少种不同的字符串。

$2\le |S|\le 30$，$0\le K\le 10^9$，$S$ 只包含字符 `K`、`E`、`Y`。

```input1
KEY
1
```

```output1
3
```

```input2
KKEE
2
```

```output2
4
```

```input3
KKEEYY
1000000000
```

```output3
90
```

## 提示
### 制約

- $ 2\ \leq\ |S|\ \leq\ 30 $
- $ 0\ \leq\ K\ \leq\ 10^9 $
- $ S $ は `K`, `E`, `Y` のみからなる

### Sample Explanation 1

`KEY` に対して $ 1 $ 回以下の操作を行うことで得られる文字列は `KEY`, `EKY`, `KYE` の $ 3 $ 種類です。

### Sample Explanation 2

`KKEE` に対して $ 2 $ 回以下の操作を行うことで得られる文字列は `KKEE`, `KEKE`, `EKKE`, `KEEK` の $ 4 $ 種類です。

