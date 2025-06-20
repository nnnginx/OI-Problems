# AT_abc292_d [ABC292D] Unicyclic Components

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc292/tasks/abc292_d

頂点に $ 1 $ から $ N $ の番号が、辺に $ 1 $ から $ M $ の番号がついた $ N $ 頂点 $ M $ 辺の無向グラフが与えられます。辺 $ i $ は頂点 $ u_i $ と頂点 $ v_i $ を結んでいます。

このグラフのすべての連結成分が次の条件を満たすかどうかを判定してください。

- その連結成分に含まれる頂点の個数と辺の本数が等しい。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ u_1 $ $ v_1 $ $ \vdots $ $ u_M $ $ v_M $

## 输出格式

すべての連結成分が条件を満たすならば `Yes` と、そうでなければ `No` と出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 3
2 3
1 1
2 3
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
5 5
1 2
2 3
3 4
3 5
1 5
```

### 输出 #2

```
Yes
```

## 输入输出样例 #3

### 输入 #3

```
13 16
7 9
7 11
3 8
1 13
11 11
6 11
8 13
2 11
3 3
8 12
9 11
1 11
5 13
3 12
6 9
1 10
```

### 输出 #3

```
No
```

## 说明/提示

### 注釈

**無向グラフ** とは、辺に向きの無いグラフのことをいいます。  
あるグラフの **部分グラフ** とは、元のグラフのいくつかの頂点といくつかの辺を選んでできるグラフのことをいいます。  
グラフが **連結** であるとは、グラフに含まれるすべての頂点同士が辺を経由して互いに行き来できることをいいます。  
**連結成分** とは、連結な部分グラフのうち、そのグラフを含んだより大きい連結な部分グラフが存在しないものをいいます。

### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 0\ \leq\ M\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ u_i\ \leq\ v_i\ \leq\ N $
- 入力はすべて整数

### Sample Explanation 1

このグラフには頂点 $ 1 $ のみからなる連結成分と頂点 $ 2,3 $ からなる連結成分があります。 前者には $ 1 $ 本の辺(辺 $ 2 $ )が、後者には $ 2 $ 本の辺(辺 $ 1,3 $ )が含まれており、条件を満たします。