## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc257/tasks/abc257_a

`A` を $ N $ 個、`B` を $ N $ 個、…、`Z` を $ N $ 個この順に繋げて得られる文字列の先頭から $ X $ 番目の文字を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ X $

## 输出格式
答えを出力せよ。

## 题目大意
有 $A、B、...、Z$ 各 $N$ 个，按顺序连接成字符串，并求出该字符串的第 $X$ 个字母是什么。

```input1
1 3
```

```output1
C
```

```input2
2 12
```

```output2
F
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ 1\ \leq\ X\ \leq\ N\times\ 26 $
- 入力は全て整数

### Sample Explanation 1

得られる文字列は `ABCDEFGHIJKLMNOPQRSTUVWXYZ` です。先頭から $ 3 $ 番目の文字は `C` です。

### Sample Explanation 2

得られる文字列は `AABBCCDDEEFFGGHHIIJJKKLLMMNNOOPPQQRRSSTTUUVVWWXXYYZZ` です。先頭から $ 12 $ 番目の文字は `F` です。

