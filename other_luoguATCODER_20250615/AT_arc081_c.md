# AT_arc081_c [ARC081E] Don't Be a Subsequence

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc081/tasks/arc081_c

文字列 $ S $ に対して，その文字列を構成する文字を $ 0 $ 文字以上取り除き，残った文字を元の順番で並べて得られる文字列を $ S $ の部分列と呼びます． たとえば，`arc` や `artistic` や (空文字列) は `artistic` の部分列ですが，`abc` や `ci` は `artistic` の部分列ではありません．

英小文字からなる文字列 $ A $ が与えられます． このとき，英小文字からなる文字列で，$ A $ の部分列ではないようなもののうち，最も短いものを求めてください． ただし，そのようなものが複数ある場合には，辞書順で最小のものを求めてください．

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ A $

## 输出格式

英小文字からなる $ A $ の部分列でないような最短の文字列のうち，辞書順最小のものを出力せよ．

## 输入输出样例 #1

### 输入 #1

```
atcoderregularcontest
```

### 输出 #1

```
b
```

## 输入输出样例 #2

### 输入 #2

```
abcdefghijklmnopqrstuvwxyz
```

### 输出 #2

```
aa
```

## 输入输出样例 #3

### 输入 #3

```
frqnvhydscshfcgdemurlfrutcpzhopfotpifgepnqjxupnskapziurswqazdwnwbgdhyktfyhqqxpoidfhjdakoxraiedxskywuepzfniuyskxiyjpjlxuqnfgmnjcvtlpnclfkpervxmdbvrbrdn
```

### 输出 #3

```
aca
```

## 说明/提示

### 制約

- $ 1\ \leq\ |A|\ \leq\ 2\ \times\ 10^5 $
- $ A $ は英小文字のみからなる．

### Sample Explanation 1

`atcoderregularcontest` という文字列は `a` を部分列として含みますが，`b` は含みません．