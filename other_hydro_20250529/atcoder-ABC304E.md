## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc304/tasks/abc304_e

$ N $ 頂点 $ M $ 辺の無向グラフ $ G $ が与えられます。 $ i\ =\ 1,\ 2,\ \ldots,\ M $ について、$ i $ 番目の辺は頂点 $ u_i $ と頂点 $ v_i $ を結ぶ無向辺です。

$ N $ 頂点のグラフは、すべての $ i\ =\ 1,\ 2,\ \ldots,\ K $ について下記の条件が成り立つとき、**良いグラフ**と呼ばれます。

- $ G $ 上で頂点 $ x_i $ と頂点 $ y_i $ を結ぶパスが存在しない。
 
与えられるグラフ $ G $ は良いグラフです。

$ Q $ 個の独立な質問が与えられるので、それらすべてに答えてください。 $ i\ =\ 1,\ 2,\ \ldots,\ Q $ について、$ i $ 番目の質問は

- 入力で与えられたグラフ $ G $ に頂点 $ p_i $ と頂点 $ q_i $ を結ぶ無向辺を $ 1 $ 本追加して得られるグラフ $ G^{(i)} $ は良いグラフですか？
 
という質問です。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ u_1 $ $ v_1 $ $ u_2 $ $ v_2 $ $ \vdots $ $ u_M $ $ v_M $ $ K $ $ x_1 $ $ y_1 $ $ x_2 $ $ y_2 $ $ \vdots $ $ x_K $ $ y_K $ $ Q $ $ p_1 $ $ q_1 $ $ p_2 $ $ q_2 $ $ \vdots $ $ p_Q $ $ q_Q $

## 输出格式
$ Q $ 行出力せよ。 $ i\ =\ 1,\ 2,\ \ldots,\ Q $ について、$ i $ 行目には $ i $ 番目の質問に対する答えを出力せよ。 具体的には、グラフ $ G^{(i)} $ が良いグラフである場合は `Yes` を、良いグラフでない場合は `No` を出力せよ。

## 题目大意
### 题目描述

给定无向图 $ G $，其包含 $ N $ 个顶点和 $ M $ 条边。对于 $ i = 1, 2, \dots, M $，第 $ i $ 条边连接着结点 $ u_i $ 与结点 $ v_i $。

如果图 $ G $ 满足以下条件：

- 对于所有 $ i = 1, 2, \dots, K $，结点 $ x_i $ 与结点 $ y_i $ 之间**均没有**路径连接。

则称图 $ G $ 是一张**好图**。

给定 $ Q $ 个**独立**的询问，请你逐个回答。对于 $ i = 1, 2, \dots, Q $，第 $ i $ 次询问内容如下：

- 在图 $ G $ 上添加一条连接着结点 $ p_i $ 与结点 $ q_i $ 的无向边，由此得到的新图 $ G^{(i)} $ 是否是一张好图？

### 样例解释

- 对于第一次询问，图 $ G^{(1)} $ 不是一张好图，因为该图存在连接着结点 $ x_1 = 1 $ 与结点 $ y_1 = 5 $ 的路径 $ 1 \to 2 \to 5 $。因此，输出`No`。
- 对于第二次询问，图 $ G^{(2)} $ 不是一张好图，因为该图存在连接着结点 $ x_2 = 2 $ 与结点 $ y_2 = 6 $ 的路径 $ 2 \to 6 $。因此，输出`No`。
- 对于第三次询问，图 $ G^{(3)} $ 是一张好图。因此，输出`Yes`。
-  对于第四次询问，图 $ G^{(4)} $ 是一张好图。因此，输出`Yes`。

正如样例所示，给定的图 $ G $ 可能存在自环与重边。

```input1
6 6
1 2
2 3
2 3
3 1
5 4
5 5
3
1 5
2 6
4 3
4
2 5
2 6
5 6
5 4
```

```output1
No
No
Yes
Yes
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 0\ \leq\ M\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ u_i,\ v_i\ \leq\ N $
- $ 1\ \leq\ K\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ x_i,\ y_i\ \leq\ N $
- $ x_i\ \neq\ y_i $
- $ i\ \neq\ j\ \implies\ \lbrace\ x_i,\ y_i\ \rbrace\ \neq\ \lbrace\ x_j,\ y_j\ \rbrace $
- すべての $ i\ =\ 1,\ 2,\ \ldots,\ K $ について次が成り立つ：頂点 $ x_i $ と頂点 $ y_i $ を結ぶパスは存在しない。
- $ 1\ \leq\ Q\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ p_i,\ q_i\ \leq\ N $
- $ p_i\ \neq\ q_i $
- 入力はすべて整数
 
### Sample Explanation 1

\- $ 1 $ 番目の質問に関して、グラフ $ G^{(1)} $ は良いグラフではありません。なぜなら、頂点 $ x_1\ =\ 1 $ と頂点 $ y_1\ =\ 5 $ を結ぶパス $ 1\ \rightarrow\ 2\ \rightarrow\ 5 $ を持つからです。よって、`No` と出力します。 - $ 2 $ 番目の質問に関して、グラフ $ G^{(2)} $ は良いグラフではありません。なぜなら、頂点 $ x_2\ =\ 2 $ と頂点 $ y_2\ =\ 6 $ を結ぶパス $ 2\ \rightarrow\ 6 $ を持つからです。よって、`No` と出力します。 - $ 3 $ 番目の質問に関して、グラフ $ G^{(3)} $ は良いグラフです。よって、`Yes` と出力します。 - $ 4 $ 番目の質問に関して、グラフ $ G^{(4)} $ は良いグラフです。よって、`Yes` と出力します。 この入力例のように、与えられるグラフ $ G $ が自己ループや多重辺を持つ場合があることに注意してください。

