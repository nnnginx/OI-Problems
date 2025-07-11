# AT_utpc2021_i Card Decks

## 题目描述

[problemUrl]: https://atcoder.jp/contests/utpc2021/tasks/utpc2021_i

$ 1 $ から $ M $ までの数が一つずつ書かれた $ M $ 枚のカードからなる山札が $ N $ 個あります。 $ i $ 個目の山札の上から $ j $ 枚目には、 $ a_{i,\ j} $ が書かれています。

あなたはこれらの山札に対して、以下の $ 2 $ 種類の操作をそれぞれ好きな順に何度でも行うことができます。

- 操作 $ 1 $：山札を $ 1 $ つ選び、一番上のカードを、同じ山札の一番下に移動させる。
- 操作 $ 2 $：$ N $ 個の山札の一番上のカードに書かれている数が全て同じなら、それらを全て取って食べる。

全てのカードを食べるために必要な操作 $ 1 $ の回数の最小値はいくつですか？

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ a_{1,\ 1} $ $ \ldots $ $ a_{1,\ M} $ $ \vdots $ $ a_{N,\ 1} $ $ \ldots $ $ a_{N,\ M} $

## 输出格式

答えを $ 1 $ 行に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4 3
2 3 1
1 2 3
2 1 3
3 2 1
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
7 6
1 2 3 4 5 6
3 5 6 1 4 2
2 5 4 3 6 1
5 1 2 4 6 3
3 2 6 5 4 1
4 1 2 5 3 6
6 5 4 3 1 2
```

### 输出 #2

```
35
```

## 说明/提示

### 制約

- 入力は全て整数
- $ 1\ \le\ N\ \le\ 2\ \times\ 10^5 $
- $ 1\ \le\ M\ \le\ 22 $
- $ 1\ \leq\ a_{i,\ j}\ \leq\ M $
- $ a_{i,\ j}\ \neq\ a_{i,\ k} $ $ (j\ \neq\ k) $

### 部分点

- $ 1\ \le\ M\ \le\ 16 $ を満たすデータセットに正解した場合は $ 30 $ 点が与えられる。

### Sample Explanation 1

次のように操作を行えばよいです。 - 山札 $ 2 $ に対して操作 $ 1 $ を行う。 - 山札 $ 4 $ に対して操作 $ 1 $ を行う。 - 操作 $ 2 $ を行う。（全ての山札の一番上のカードは $ 2 $ である。） - 山札 $ 1 $ に対して操作 $ 1 $ を行う。 - 山札 $ 2 $ に対して操作 $ 1 $ を行う。 - 操作 $ 2 $ を行う。（全ての山札の一番上のカードは $ 1 $ である。） - 操作 $ 2 $ を行う。（全ての山札の一番上のカードは $ 3 $ である。）