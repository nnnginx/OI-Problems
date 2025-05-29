## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc054/tasks/abc054_c

自己ループと二重辺を含まない $ N $ 頂点 $ M $ 辺の重み無し無向グラフが与えられます。  
 $ i\ (1≦i≦M) $ 番目の辺は頂点 $ a_i $ と頂点 $ b_i $ を結びます。   
 ここで、自己ループは $ a_i\ =\ b_i\ (1≦i≦M) $ となる辺のことを表します。   
 また、二重辺は $ a_i=a_j $ かつ $ b_i=b_j\ (1≦i\ <\ j≦M) $ となる辺のことを表します。   
 頂点 $ 1 $ を始点として、全ての頂点を1度だけ訪れるパスは何通りありますか。   
 ただし、パスの始点と終点の頂点も訪れたものとみなします。

例として、図1のような無向グラフが与えられたとします。

 ![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc054_c/5764771c0b3041c3346efe47c98edb49c94a9b3d.png)図1：無向グラフの例

 

このとき、図2で表されるパスは条件を満たします。

 ![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc054_c/7f5174784cef5e6da48aed9eeb9756a6de9199db.png)図2：条件を満たすパスの例

 

しかし、図3で表されるパスは条件を満たしません。全ての頂点を訪れていないからです。

 ![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc054_c/ad6e861039122f07481a4ef820a2461de4e5e54c.png)図3：条件を満たさないパスの例1

 

また、図4で表されるパスも条件を満たしません。始点が頂点 $ 1 $ ではないからです。

 ![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc054_c/ad37aa02ed59054ab7ef974821bffd978f95285d.png)図4：条件を満たさないパスの例2

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ a_1 $ $ b_1 $ $ a_2 $ $ b_2 $ $ : $ $ a_M $ $ b_M $

## 输出格式
問題文の条件を満たすパスが何通りあるか出力せよ。

## 题目大意
#### 题目描述

给定一个没有重边和自环的 $N$ 个点 $M$ 条边的无权无向图，第 $i$ 条边连接顶点 $a _ i$ 和 $b _ i$。

求以顶点 $1$ 为起点，只访问 $1$ 次所有顶点的路径有多少条？特别地，起点和终点也视为被访问。

#### 输入格式

第一行两个整数 $N, M$。

接下来 $m$ 行，其中第 $i$ 行两个整数 $a _ i, b _ i$。

$
N M \\
a _ 1 b _ 1 \\
a _ 2 b _ 2 \\
\kern {0.667 em} \vdots \\
a _ M b _ M
$

#### 输出格式

输出满足条件的路径有多少。

#### 数据范围

$
2 \le N \le 8 \\
0 \le M \le N(N - 1) \\
1 \le a _ i < b _ i \le N
$

给定的无向图中不包含重边和自环。

```input1
3 3
1 2
1 3
2 3
```

```output1
2
```

```input2
7 7
1 3
2 7
3 4
4 5
4 6
5 6
6 7
```

```output2
1
```

## 提示
### 制約

- $ 2≦N≦8 $
- $ 0≦M≦N(N-1)/2 $
- $ 1≦a_i\ <\ b_i≦N $
- 与えられるグラフは自己ループと二重辺を含まない。

### Sample Explanation 1

与えられるグラフは以下の図で表されます。 !\[43c0ac53de20d989d100bf60b3cd05fa.png\](https://atcoder.jp/img/5013/43c0ac53de20d989d100bf60b3cd05fa.png) 条件を満たすパスは以下の $ 2 $ 通りです。 !\[c4a27b591d364fa479314e3261b85071.png\](https://atcoder.jp/img/5013/c4a27b591d364fa479314e3261b85071.png)

### Sample Explanation 2

このテストケースは問題文の例と同じです。

