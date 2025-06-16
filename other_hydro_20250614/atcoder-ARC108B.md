## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc108/tasks/arc108_b

長さ $ N $ の英小文字のみからなる文字列 $ s $ が与えられます。 すぬけ君は $ s $ から `fox` という部分文字列を $ 1 $ つ選んで取り除き、その前後の部分を連結する、という操作を何度でも行うことができます。

すぬけ君が操作を何度か行ったあと、$ s $ の長さは最小でいくつになりえますか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ s $

## 输出格式
すぬけ君が操作を何度か行ったあとの $ s $ の長さとしてありうる値の最小値を出力せよ。

## 题目大意
输入一个长度为n的字符串，如果这个字符串有“fox”，则删除，最后输出经过删除的字符串的长度。

```input1
6
icefox
```

```output1
3
```

```input2
7
firebox
```

```output2
7
```

```input3
48
ffoxoxuvgjyzmehmopfohrupffoxoxfofofoxffoxoxejffo
```

```output3
27
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^{5} $
- $ s $ は英小文字のみからなる長さ $ N $ の文字列

### Sample Explanation 1

\- `icefox` の末尾 `fox` を取り除くことで $ s $ を `ice` にすることができます。

### Sample Explanation 2

\- `fox` という部分文字列が存在しません。

