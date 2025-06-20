# AT_abc282_b [ABC282B] Let's Get a Perfect Score

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc282/tasks/abc282_b

$ 1 $ から $ N $ までの番号がついた $ N $ 人の参加者が、$ 1 $ から $ M $ までの番号がついた $ M $ 問からなるコンテストに参加します。

$ 1 $ 以上 $ N $ 以下の整数 $ i $ 、$ 1 $ 以上 $ M $ 以下の整数 $ j $ について、$ S_i $ の $ j $ 番目の文字が `o` のとき参加者 $ i $ は問題 $ j $ を解くことが可能で、$ S_i $ の $ j $ 番目の文字が `x` のとき参加者 $ i $ は問題 $ j $ を解くことが不可能です。

このコンテストは、二人の参加者でペアを組んで参加します。二人が協力することで $ M $ 問全てを解くことが可能であるようなペアの個数を答えてください。

より厳密には、$ 1\leq\ x\ <\ y\leq\ N $ を満たす整数の組 $ (x,y) $ であって、 $ 1 $ 以上 $ M $ 以下の任意の整数 $ j $ について、参加者 $ x $ か参加者 $ y $ の少なくとも一方は問題 $ j $ を解くことが可能であるという条件を満たすものの個数を答えてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 5
ooooo
oooxx
xxooo
oxoxo
xxxxx
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
3 2
ox
xo
xx
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
2 4
xxxx
oxox
```

### 输出 #3

```
0
```

## 说明/提示

### 制約

- $ N $ は $ 2 $ 以上 $ 30 $ 以下の整数
- $ M $ は $ 1 $ 以上 $ 30 $ 以下の整数
- $ S_i $ は `o`, `x` からなる長さ $ M $ の文字列
 
### Sample Explanation 1

参加者 $ 1 $ と $ 2 $ のペア、参加者 $ 1 $ と $ 3 $ のペア、参加者 $ 1 $ と $ 4 $ のペア、参加者 $ 1 $ と $ 5 $ のペア、参加者 $ 2 $ と $ 3 $ のペアの $ 5 $ 個のペアが条件を満たします。 例えば参加者 $ 2 $ と $ 4 $ のペアは、問題 $ 4 $ が解けないので条件を満たしません。