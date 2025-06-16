# AT_abc029_b [ABC029B] カキ

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc029/tasks/abc029_b

英小文字からなる $ 12 $ 個の文字列 $ S_1 $, $ S_2 $, ..., $ S_{12} $ が入力されます。  
これらの文字列のうち、文字 `r` が含まれるものの個数を数えてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S_1 $ $ S_2 $ : $ S_{12} $

- $ i $ 行目 ($ 1 $ $ ≦ $ $ i $ $ ≦ $ $ 12 $) に、英小文字からなる文字列 $ S_i $ ($ 1 $ $ ≦ $ $ |S_i| $ $ ≦ $ $ 10 $) が与えられる。  
  これらの文字列はすべて異なる。

## 输出格式

標準出力に、 $ 12 $ 個の文字列 $ S_1 $, $ S_2 $, ..., $ S_{12} $ のうち文字 `r` が含まれるものの個数を出力し、最後に改行せよ。   
`r` を複数個含む文字列は一度だけ数える。

## 输入输出样例 #1

### 输入 #1

```
january
february
march
april
may
june
july
august
september
october
november
december
```

### 输出 #1

```
8
```

## 输入输出样例 #2

### 输入 #2

```
rrrrrrrrrr
srrrrrrrrr
rsr
ssr
rrs
srsrrrrrr
rssrrrrrr
sss
rrr
srr
rsrrrrrrrr
ssrrrrrrrr
```

### 输出 #2

```
11
```

## 说明/提示

### Sample Explanation 1

$ S_1 $, $ S_2 $, $ S_3 $, $ S_4 $, $ S_9 $, $ S_{10} $, $ S_{11} $, $ S_{12} $ の $ 8 $ 個の文字列に文字 `r` が含まれています。 $ S_2 $ には `r` が $ 2 $ 回出現していますが、一度しか数えません。