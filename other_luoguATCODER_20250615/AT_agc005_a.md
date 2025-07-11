# AT_agc005_a [AGC005A] STring

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc005/tasks/agc005_a

文字列 $ X $ が与えられます。$ X $ の長さは偶数であり、半分は `S` 、もう半分は `T` からなります。

高橋君は `ST` という文字列が苦手です。なので以下の操作を $ 10^{10000} $ 回行うことにしました。

- $ X $ の(連続な)部分文字列で `ST` となるもののうち、最も左側にあるものを取り除く。存在しないならば何もしない。

最終的に $ X $ は何文字になるかを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ X $

## 输出格式

$ 1 $ 行に問題の答えを出力する。

## 输入输出样例 #1

### 输入 #1

```
TSTTSS
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
SSTTST
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
TSSTTTSS
```

### 输出 #3

```
4
```

## 说明/提示

### 制約

- $ 2\ ≦\ |X|\ ≦\ 200,000 $
- $ X $ の長さは偶数
- $ X $ を構成する文字のうち半分は `S` であり、もう半分は `T` である

### 部分点

- $ 200 $ 点分のデータセットでは $ |X|\ ≦\ 200 $ が成り立つ

### Sample Explanation 1

$ 1 $ 回目の操作では `TSTTSS` の $ 2,3 $ 文字目が `ST` なので取り除きます。 $ X $ は `TTSS` になり、もう `ST` はないため残り $ 10^{10000}-1 $ 回は何もしません。 よって答えは $ 4 $ となります。

### Sample Explanation 2

`SSTTST` ⇒ `STST` ⇒ `ST` ⇒ `` となり、最終的に空文字列になります。

### Sample Explanation 3

`TSSTTTSS` ⇒ `TSTTSS` ⇒ `TTSS` となります。