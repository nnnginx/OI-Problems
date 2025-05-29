## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc060/tasks/abc060_a

文字列 $ A $, $ B $, $ C $ が与えられます。これがしりとりになっているか判定してください。

つまり、

- $ A $ の最後の文字と $ B $ の最初の文字が同じ
- $ B $ の最後の文字と $ C $ の最初の文字が同じ

この $ 2 $ つが正しいか判定してください。

両方とも正しいならば `YES`、そうでないならば `NO` を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ C $

## 输出格式
`YES` か `NO` を出力する。

## 题目大意
# 输入格式

第一行 三个字符串 $A$,$B$,$C$（$1\le |A|,|B|,|C|\le10$）。

# 输出格式

如果这三个字符串构成接龙（即下一个单词的首字母 和当前单词的尾字母相同），输出 `YES`，否则输出 `NO`。

**结尾记得换行！**

```input1
rng gorilla apple
```

```output1
YES
```

```input2
yakiniku unagi sushi
```

```output2
NO
```

```input3
a a a
```

```output3
YES
```

```input4
aaaaaaaaab aaaaaaaaaa aaaaaaaaab
```

```output4
NO
```

## 提示
### 制約

- $ A,\ B,\ C $ は全て英小文字(`a` ~ `z`)からなる。
- $ 1\ ≦\ |A|,\ |B|,\ |C|\ ≦\ 10 $
- なお、$ |A|,\ |B|,\ |C| $ は文字列 $ A,\ B,\ C $ の長さを表します。

### Sample Explanation 1

これはしりとりになっています。

### Sample Explanation 2

$ A $ と $ B $ はしりとりになっていますが、$ B $ と $ C $ がしりとりになっていません。

