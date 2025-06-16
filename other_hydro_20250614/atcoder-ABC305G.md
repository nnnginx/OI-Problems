## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc305/tasks/abc305_g

`a`, `b` からなる長さ $ 6 $ 以下の空でない文字列の集合 $ S=\lbrace\ s\ _\ 1,s\ _\ 2,\ldots,s\ _\ M\rbrace $ が与えられます。 以下の条件を満たす `a`, `b` からなる長さ $ N $ の文字列 $ T $ はいくつあるか求めてください。

- 任意の $ s\ _\ i\in\ S $ に対して、$ T $ は $ s\ _\ i $ を連続する部分文字列として含まない
 
ただし、答えは非常に大きくなる可能性があるので、答えを $ 998244353 $ で割った余りを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ s\ _\ 1 $ $ s\ _\ 2 $ $ \vdots $ $ s\ _\ M $

## 输出格式
答えを $ 998244353 $ で割ったあまりを $ 1 $ 行で出力せよ。

## 题目大意
### 题目描述

给定一个由 $M$ 个长度不超过 $6$ 的仅由字母 $\texttt a$ 和 $\texttt b$ 组成的非空字符串集合 $S=\{s_1, s_2, ..., s_M\}$。

求有多少个字符串 $T$ 满足以下条件：

- 长度为 $N$ 且仅由字母 $\texttt a$ 和 $\texttt b$ 组成。
- 对于任意 $s_i\in S$，$T$ 中不包含 $s_i$ 作为连续的子串。

由于答案可能很大，所以对 $998244353$ 取模。

### 数据范围

$1\leq N\leq 10^{18}$

$1\leq M\leq 126$

$N$ 和 $M$ 是整数。

$s_i$ 是由字母 $a$ 和 $b$ 组成的长度不超过 $6$ 的非空字符串。

$s_i \neq s_j$（$1\leq i<j\leq M$）。

### 输入格式
输入共 $M+1$ 行，第一行包括两个整数 $N$ 和 $M$，表示字符串长度和非空字符串集合大小。接下来 $M$ 行，每行一个字符串 $s_i$。

### 输出格式
输出仅包含一个整数，表示满足条件的字符串 $T$ 的个数对 $998244353$ 取模后的结果。

```input1
4 3
aab
bbab
abab
```

```output1
10
```

```input2
20 1
aa
```

```output2
17711
```

```input3
1000000007 28
bbabba
bbbbaa
aabbab
bbbaba
baaabb
babaab
bbaaba
aabaaa
aaaaaa
aabbaa
bbaaaa
bbaabb
bbabab
aababa
baaaba
ababab
abbaba
aabaab
ababaa
abbbba
baabaa
aabbbb
abbbab
baaaab
baabbb
ababbb
baabba
abaaaa
```

```output3
566756841
```

## 提示
### 制約

- $ 1\leq\ N\leq10^{18} $
- $ 1\leq\ M\leq126 $
- $ N,M $ は整数
- $ s\ _\ i $ は `a`, `b` からなる長さ $ 6 $ 以下の空でない文字列
- $ s\ _\ i\neq\ s\ _\ j\ (1\leq\ i\lt\ j\leq\ M) $
 
### Sample Explanation 1

`a`, `b` からなる長さ $ 4 $ の文字列で、連続する部分列として `aab`, `bbab`, `abab` をもたないようなものは `aaaa`, `abaa`, `abba`, `abbb`, `baaa`, `baba`, `babb`, `bbaa`, `bbba`, `bbbb` の $ 10 $ 個なので、$ 10 $ を出力してください。

### Sample Explanation 3

$ 998244353 $ で割ったあまりを出力してください。

