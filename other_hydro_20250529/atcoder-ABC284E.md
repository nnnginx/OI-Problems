## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc284/tasks/abc284_e

頂点に $ 1 $ から $ N $ の番号が、辺に $ 1 $ から $ M $ の番号がついた $ N $ 頂点 $ M $ 辺の単純無向グラフが与えられます。辺 $ i $ は頂点 $ u_i $ と頂点 $ v_i $ を結んでいます。また、各頂点の次数は $ 10 $ 以下です。  
 頂点 $ 1 $ を始点とする単純パス(同じ頂点を複数回通らないパス)の個数を $ K $ とします。$ \min(K,\ 10^6) $ を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ u_1 $ $ v_1 $ $ u_2 $ $ v_2 $ $ \vdots $ $ u_M $ $ v_M $

## 输出格式
答えを出力せよ。

## 题目大意
给定一张 $N$ 个节点 $M$ 条边的无向图，保证每个节点的度数 $\le 10$。

记从任意节点回到 $1$ 号点的不同路径总数为 $K$，请输出 $\min(K,10^6)$。

翻译 by @Mars\_Dingdang

```input1
4 2
1 2
2 3
```

```output1
3
```

```input2
4 6
1 2
1 3
1 4
2 3
2 4
3 4
```

```output2
16
```

```input3
8 21
2 6
1 3
5 6
3 8
3 6
4 7
4 6
3 4
1 5
2 4
1 2
2 7
1 4
3 5
2 5
2 3
4 5
3 7
6 7
5 7
2 8
```

```output3
2023
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 0\ \leq\ M\ \leq\ \min\ \left(2\ \times\ 10^5,\ \frac{N(N-1)}{2}\right) $
- $ 1\ \leq\ u_i,\ v_i\ \leq\ N $
- 入力で与えられるグラフは単純グラフ
- 入力で与えられるグラフの頂点の次数はすべて $ 10 $ 以下
- 入力される値は全て整数
 
### Sample Explanation 1

条件を満たすパスは次の $ 3 $ 個です。(長さが $ 0 $ のパスも数えるのに注意してください。) - 頂点 $ 1 $ - 頂点 $ 1 $, 頂点 $ 2 $ - 頂点 $ 1 $, 頂点 $ 2 $, 頂点 $ 3 $

