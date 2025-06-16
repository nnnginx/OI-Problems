## 题目描述
[problemUrl]: https://atcoder.jp/contests/diverta2019/tasks/diverta2019_c

すぬけ君は $ N $ 個の文字列を持っています。$ i $ 番目の文字列は $ s_i $ です。

これらの文字列を好きな順序で並べたあと、連結して $ 1 $ つの文字列を作ることを考えます。 作った文字列に `AB` という部分文字列が含まれる個数としてありうる値のうち、最大値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ s_1 $ $ \vdots $ $ s_N $

## 输出格式
答えを出力せよ。

## 题目大意
Snuke 有 $N$ 个字符串。 第 $i$ 个字符串是 $s_i$。

在以某种顺序排列它们之后，让我们将这些字符串连接成一个字符串。 在结果字符串中找到 `AB` 的最大可能出现次数。

```input1
3
ABCA
XBAZ
BAD
```

```output1
2
```

```input2
9
BEWPVCRWH
ZZNQYIJX
BAVREA
PA
HJMYITEOX
BCJHMRMNK
BP
QVFABZ
PRGKSPUNA
```

```output2
4
```

```input3
7
RABYBBE
JOZ
BMHQUVA
BPA
ISU
MCMABAOBHZ
SZMEHMA
```

```output3
4
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^{4} $
- $ 2\ \leq\ |s_i|\ \leq\ 10 $
- $ s_i $ は英大文字のみからなる

### Sample Explanation 1

\- 例えば、`ABCA`, `BAD`, `XBAZ` の順で連結して `ABCABADXBAZ` を作ったとき、`AB` という部分文字列は $ 2 $ つ含まれます。

