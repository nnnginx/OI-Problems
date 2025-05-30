## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc266/tasks/abc266_f

頂点に $ 1 $ から $ N $ の番号がついた $ N $ 頂点 $ N $ 辺の連結な単純無向グラフ $ G $ が与えられます。$ i $ 番目の辺は頂点 $ u_i $ と頂点 $ v_i $ を双方向に結んでいます。

以下の $ Q $ 個のクエリに答えてください。

- 頂点 $ x_i $ から頂点 $ y_i $ に向かう単純パス（同じ頂点を $ 2 $ 度通らないパス）が一意に定まるか判定せよ。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ u_1 $ $ v_1 $ $ u_2 $ $ v_2 $ $ \vdots $ $ u_N $ $ v_N $ $ Q $ $ x_1 $ $ y_1 $ $ x_2 $ $ y_2 $ $ \vdots $ $ x_Q $ $ y_Q $

## 输出格式
$ Q $ 行出力せよ。

$ i\ (1\ \leq\ i\ \leq\ Q) $ 行目には、頂点 $ x_i $ から頂点 $ y_i $ に向かう単純パスが一意に定まる場合 `Yes`、そうでない場合 `No` を出力せよ。

## 题目大意
### 题目描述

给定一张有 $N$ 个点、$N$ 条边的简单连通无向图和 $Q$ 次询问，对于每次询问，给定 $x_i,y_i$，表示两点的编号，请你回答第 $x_i$ 个点和第 $y_i$ 个点之间是否**有且仅有**一条简单路径。

+ 什么是简单路径？

如果路径上的各顶点均不重复，则称这样的路径为简单路径。

### 输入格式

第一行包含一个整数 $N$；

接下来 $N$ 行，每行两个整数 $u_i,v_i$，表示第 $i$ 条边连接的两个点；

再接下来一行包含一个整数 $Q$；

最后 $Q$ 行，每行两个整数 $x_i,y_i$，含义见题目描述。

### 输出格式

对于每次询问，输出一个字符串 `Yes` 或 `No`，分别表示两点之间是否仅存在一条简单路径，每个询问分别输出一行。

### 样例

见原题面。

### 样例解析

样例 #1 解析：

对于第一次询问，从 $1$ 到 $2$ 有两条简单路径 $(1,2)$、$(1,3,2)$，所以输出 `No`。

对于第二次询问，从 $1$ 到 $4$ 仅有一条路径 $(1,4)$，所以输出 `Yes`。

对于第三次询问，从 $1$ 到 $5$ 有两条简单路径 $(1,2,5)$、$(1,3,2,5)$，所以输出 `No`。

### 数据范围

对于 $30\%$ 的数据，$N \le 100$，$Q \le \frac{N(N-1)}{2}$；

对于 $100\%$ 的数据，$3 \le N \le 2 \times 10^5$，$1 \le u_i<v_i \le N$，$1 \le Q \le 2 \times 10^5$，$1 \le x_i < y_i \le N$，保证图没有重边或自环，且给定询问均不重复。

翻译 by @CarroT1212

```input1
5
1 2
2 3
1 3
1 4
2 5
3
1 2
1 4
1 5
```

```output1
No
Yes
No
```

```input2
10
3 5
5 7
4 8
2 9
1 2
7 9
1 6
4 10
2 5
2 10
10
1 8
6 9
8 10
6 8
3 10
3 9
1 10
5 8
1 10
7 8
```

```output2
Yes
No
Yes
Yes
No
No
Yes
No
Yes
No
```

## 提示
### 制約

- $ 3\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ u_i\ <\ v_i\leq\ N $
- $ i\ \neq\ j $ ならば $ (u_i,v_i)\ \neq\ (u_j,v_j) $
- $ G $ は $ N $ 頂点 $ N $ 辺の連結な単純無向グラフ
- $ 1\ \leq\ Q\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ x_i\ <\ y_i\leq\ N $
- 入力は全て整数

### Sample Explanation 1

頂点 $ 1 $ から $ 2 $ に向かう単純パスは $ (1,2),(1,3,2) $ と一意に定まらないので、 $ 1 $ 個目のクエリの答えは `No` です。 頂点 $ 1 $ から $ 4 $ に向かう単純パスは $ (1,4) $ と一意に定まるので、$ 2 $ 個目のクエリの答えは `Yes` です。 頂点 $ 1 $ から $ 5 $ に向かう単純パスは $ (1,2,5),(1,3,2,5) $ と一意に定まらないので、$ 3 $ 個目のクエリの答えは `No` です。

