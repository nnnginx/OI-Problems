# AT_diverta2019_c AB Substrings

## 题目描述

[problemUrl]: https://atcoder.jp/contests/diverta2019/tasks/diverta2019_c

すぬけ君は $ N $ 個の文字列を持っています。$ i $ 番目の文字列は $ s_i $ です。

これらの文字列を好きな順序で並べたあと、連結して $ 1 $ つの文字列を作ることを考えます。 作った文字列に `AB` という部分文字列が含まれる個数としてありうる値のうち、最大値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ s_1 $ $ \vdots $ $ s_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
ABCA
XBAZ
BAD
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
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

### 输出 #2

```
4
```

## 输入输出样例 #3

### 输入 #3

```
7
RABYBBE
JOZ
BMHQUVA
BPA
ISU
MCMABAOBHZ
SZMEHMA
```

### 输出 #3

```
4
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 10^{4} $
- $ 2\ \leq\ |s_i|\ \leq\ 10 $
- $ s_i $ は英大文字のみからなる

### Sample Explanation 1

\- 例えば、`ABCA`, `BAD`, `XBAZ` の順で連結して `ABCABADXBAZ` を作ったとき、`AB` という部分文字列は $ 2 $ つ含まれます。