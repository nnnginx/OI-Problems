# AT_abc303_e [ABC303E] A Gift From the Stars

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc303/tasks/abc303_e

以下の条件を満たす $ k+1 $ 頂点 $ k $ 辺のグラフをレベル $ k\ (k\geq\ 2) $ の星と呼びます。

- ある $ 1 $ つの頂点が、他の $ k $ 個の頂点と $ 1 $ 本ずつ辺で結ばれている。それ以外の辺は存在しない。
 
高橋君は、はじめ何個かの星からなるグラフを持っていました。そして、以下の手続きを全てのグラフの頂点が連結になるまでくり返し行いました。

- 持っているグラフの頂点から二つの頂点を選ぶ。このとき、選んだ二つの頂点の次数は共に $ 1 $ であり、かつ選んだ二つの頂点は非連結である必要がある。選んだ二つの頂点を結ぶ辺を張る。
 
その後、高橋君は手続きが終了した後のグラフの頂点に、適当に $ 1 $ から $ N $ の番号を付けました。このグラフは木となっており、これを $ T $ と呼びます。$ T $ には $ N-1 $ 本の辺があり、 $ i $ 番目の辺は $ u_i $ と $ v_i $ を結んでいました。

その後高橋君は、はじめ持っていた星の個数とレベルを忘れてしまいました。$ T $ の情報からはじめ持っていた星の個数とレベルを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ u_1 $ $ v_1 $ $ \vdots $ $ u_{N-1} $ $ v_{N-1} $

## 输出格式

高橋君が持っていた星が $ M $ 個であり、星のレベルがそれぞれ $ L=(L_1,L_2,\ldots,L_M) $ であったとする。 このとき、$ L $ を昇順に並び替え空白区切りで出力せよ。

なお、この問題では常に解が一意に定まることが証明できる。

## 输入输出样例 #1

### 输入 #1

```
6
1 2
2 3
3 4
4 5
5 6
```

### 输出 #1

```
2 2
```

## 输入输出样例 #2

### 输入 #2

```
9
3 9
7 8
8 6
4 6
4 1
5 9
7 3
5 2
```

### 输出 #2

```
2 2 2
```

## 输入输出样例 #3

### 输入 #3

```
20
8 3
8 18
2 19
8 20
9 17
19 7
8 7
14 12
2 15
14 10
2 13
2 16
2 1
9 5
10 15
14 6
2 4
2 11
5 12
```

### 输出 #3

```
2 3 4 7
```

## 说明/提示

### 制約

- $ 3\leq\ N\leq\ 2\times\ 10^5 $
- $ 1\leq\ u_i,\ v_i\leq\ N $
- 与えられるグラフは、問題文中の手続きによって得られる $ N $ 頂点の木
- 入力は全て整数
 
### Sample Explanation 1

以下の図のように、$ 2 $ つのレベル $ 2 $ の星から $ T $ は得られます。 !\[\](https://img.atcoder.jp/abc303/59ab8e04c23d5f727300be7544b1df7e.png)