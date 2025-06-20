# AT_abc136_d [ABC136D] Gathering Children

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc136/tasks/abc136_d

マスの情報を表す、`L` と `R` で構成された文字列 $ S $ が与えられます。

文字列 $ S $ の長さを $ N $ としたとき、$ N $ 個のマスが左右一列に並んでおり、左から $ i $ 番目のマスには $ S $ の左から $ i $ 番目の文字が書かれています。

ただし、左端のマスには必ず `R`、右端のマスには必ず `L` が書かれています。

はじめ、各マスには $ 1 $ 人の子どもが居ます。

子どもたちはそれぞれ次の規則に従った移動を $ 10^{100} $ 回行います。

- 今居るマスに書かれた文字に従って $ 1 $ マス移動する。すなわち、今居るマスに書かれた文字が `L` のとき左隣のマスに、`R` のとき右隣のマスに移動する。

$ 10^{100} $ 回の移動の後に各マスに居る子どもの人数を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式

$ 10^{100} $ 回の移動の後に各マスに居る子どもの人数を左のマスから順に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
RRLRL
```

### 输出 #1

```
0 1 2 1 1
```

## 输入输出样例 #2

### 输入 #2

```
RRLLLLRLRRLL
```

### 输出 #2

```
0 3 3 0 0 0 1 1 0 2 2 0
```

## 输入输出样例 #3

### 输入 #3

```
RRRLLRLLRRRLLLLL
```

### 输出 #3

```
0 0 3 2 0 2 1 0 0 0 4 4 0 0 0 0
```

## 说明/提示

### 制約

- $ S $ は長さ $ 2 $ 以上 $ 10^5 $ 以下の文字列であり、$ S $ の各文字は `L` または `R` である。
- $ S $ の $ 1 $ 文字目は `R`、$ N $ 文字目は `L` である。

### Sample Explanation 1

\- $ 1 $ 回の移動の後に各マスに居る子どもの人数は左のマスから順に $ 0,\ 2,\ 1,\ 1,\ 1 $ 人です。 - $ 2 $ 回の移動の後に各マスに居る子どもの人数は左のマスから順に $ 0,\ 1,\ 2,\ 1,\ 1 $ 人です。 - この移動を $ 10^{100} $ 回行った後に各マスに居る子どもの人数は左のマスから順に $ 0,\ 1,\ 2,\ 1,\ 1 $ 人です。