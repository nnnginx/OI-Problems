## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc287/tasks/abc287_c

$ N $ 頂点 $ M $ 辺の単純無向グラフが与えられます。頂点には $ 1,\ 2,\ \dots,\ N $ の番号が、辺には $ 1,\ 2,\ \dots,\ M $ の番号が付けられています。  
 辺 $ i\ \,\ (i\ =\ 1,\ 2,\ \dots,\ M) $ は頂点 $ u_i,\ v_i $ を結んでいます。

このグラフがパスグラフであるか判定してください。

 単純無向グラフとは **単純無向グラフ**とは、自己ループや多重辺を含まず、辺に向きの無いグラフのことをいいます。

 パスグラフとは 頂点に $ 1,\ 2,\ \dots,\ N $ の番号が付けられた$ N $ 頂点のグラフが**パスグラフ**であるとは、$ (1,\ 2,\ \dots,\ N) $ を並べ変えて得られる数列 $ (v_1,\ v_2,\ \dots,\ v_N) $ であって、以下の条件を満たすものが存在することをいいます。 - 全ての $ i\ =\ 1,\ 2,\ \dots,\ N-1 $ に対して、頂点 $ v_i,\ v_{i+1} $ を結ぶ辺が存在する
\- 整数 $ i,\ j $ が $ 1\ \leq\ i,\ j\ \leq\ N,\ |i\ -\ j|\ \geq\ 2 $ を満たすならば、頂点 $ v_i,\ v_j $ を結ぶ辺は存在しない

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ u_1 $ $ v_1 $ $ u_2 $ $ v_2 $ $ \vdots $ $ u_M $ $ v_M $

## 输出格式
与えられたグラフがパスグラフなら `Yes`、そうでないなら `No` と出力せよ。

## 题目大意
给定一个图，判断这个图是否为一条链。

```input1
4 3
1 3
4 2
3 2
```

```output1
Yes
```

```input2
2 0
```

```output2
No
```

```input3
5 5
1 2
2 3
3 4
4 5
5 1
```

```output3
No
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 0\ \leq\ M\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ u_i,\ v_i\ \leq\ N\ \,\ (i\ =\ 1,\ 2,\ \dots,\ M) $
- 入力される値は全て整数
- 入力で与えられるグラフは単純
 
### Sample Explanation 1

与えらえたグラフは下図のようであり、これはパスグラフです。 !\[example\_00\](https://img.atcoder.jp/abc287/59d45566ae7f7fd4df9801eb0fdbea5f.png)

### Sample Explanation 2

与えらえたグラフは下図のようであり、これはパスグラフではありません。 !\[example\_01\](https://img.atcoder.jp/abc287/6c608de40ba7875deaf1aa168c7f8c83.png)

### Sample Explanation 3

与えらえたグラフは下図のようであり、これはパスグラフではありません。 !\[example\_02\](https://img.atcoder.jp/abc287/73f11a6a7687f4e373da69426883e134.png)

