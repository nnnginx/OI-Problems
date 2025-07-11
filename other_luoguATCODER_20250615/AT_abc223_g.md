# AT_abc223_g [ABC223G] Vertex Deletion

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc223/tasks/abc223_g

$ N $ 頂点の木が与えられます。頂点には $ 1,2,\ldots\ ,N $ の番号がついており、$ i\,(1\ \leq\ i\ \leq\ N-1) $ 本目の辺は頂点 $ u_i $ と頂点 $ v_i $ を結んでいます。

以下の条件を満たす整数 $ i\,(1\ \leq\ i\ \leq\ N) $ の個数を求めてください。

- 元の木から頂点 $ i $ およびそれに接続する全ての辺を削除して得られるグラフの最大マッチングの大きさが、元の木の最大マッチングの大きさに等しい。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ u_1 $ $ v_1 $ $ u_2 $ $ v_2 $ $ \vdots $ $ u_{N-1} $ $ v_{N-1} $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
1 2
2 3
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
2
1 2
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
6
2 5
3 5
1 4
4 5
4 6
```

### 输出 #3

```
4
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ u_i\ <\ v_i\ \leq\ N $
- 与えられるグラフは木
- 入力は全て整数

### Sample Explanation 1

元の木の最大マッチングの大きさは $ 1 $ です。 頂点 $ 1 $ およびそれに接続する全ての辺を削除して得られるグラフの最大マッチングの大きさは $ 1 $、 頂点 $ 2 $ およびそれに接続する全ての辺を削除して得られるグラフの最大マッチングの大きさは $ 0 $、 頂点 $ 3 $ およびそれに接続する全ての辺を削除して得られるグラフの最大マッチングの大きさは $ 1 $ です。$ i=1,3 $ の $ 2 $ つが条件を満たすので、$ 2 $ を出力します。