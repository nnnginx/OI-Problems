## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc056/tasks/agc056_f

整数 $ N $ と $ M $ が与えられます． 以下の手順で生成されうる整数列 $ a=(a_1,a_2,\cdots,a_N) $ の個数を $ 998244353 $ で割った余りを求めてください．

- $ N $ 頂点，$ M $ 辺からなる連結な無向グラフ $ G $ を用意する． ここで，$ G $ は自己ループを含んではならないが，**多重辺を含んでもよい**．
- $ G $ 上で DFS を行い，$ i $ ($ 1\ \leq\ i\ \leq\ N $) 番目に訪れた頂点の次数を $ a_i $ とする． より正確には，以下の疑似コードを実行して $ a $ を得る．
 
```
a = empty array

dfs(v):
    visited[v]=True
    a.append(degree[v])
    for u in g[v]:
        if not visited[u]:
            dfs(u)

dfs(arbitrary root)
```

ここで，変数 $ g $ はグラフ $ G $ を隣接リストとして表したものであり，$ g[v] $ は頂点 $ v $ に隣接する頂点を**任意の順番**で格納したリストである．

例えば，$ N=4,M=5 $ の時，$ a=(2,4,1,3) $ を生成することは可能です． そのためには，以下のようなグラフ $ G $ を用意すればよいです．

![picture](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_agc056_f/f99de1b2bc3fc84a7273d0da5117b15b6ccf98cf.png)

ここで，頂点にかかれている数は，その頂点を DFS で何番目に訪れたかを表しています．（$ 1 $ と書かれた頂点から DFS を開始しています．） また，オレンジ色の矢印は DFS での遷移を示しており，その横の数字は辺をたどる順番を表しています．

## 输入格式
入力は以下の形式で標準入力から与えられる．

> $ N $ $ M $

## 输出格式
答えを出力せよ．

## 题目大意
### 题目描述

已知整数 $N,M$， 求有多少个整数序列 $a=(a_1,a_2,\cdots,a_N)$ 可以由以下方式生成，答案对 $998244353$ 取模。

- 选择一个 $N$ 个点，$M$ 条边的无向连通图 $G$，要求无自环，但可以有重边。
- 进行 DFS，令 $a_i$ 表示遍历到的第 $i$ 个点的度数，具体的，执行以下代码：

```
a = empty array

dfs(v):
    visited[v]=True
    a.append(degree[v])
    for u in g[v]:
        if not visited[u]:
            dfs(u)

dfs(arbitrary root)
```

这里，$g$ 是图 $G$ 的邻接表，$g[v]$ 是任意顺序的与 $v$ 相连的顶点列表。

举个例子，对于 $N=4,M=5$，一个可能的 $a=(2,4,1,3)$，图 $G$ 如下图所示：

![G](https://img.atcoder.jp/agc056/3bfec17f881ae4cd27eccae94ebeae10.png)

顶点上的数字表示访问他们的顺序，橙色箭头表示遍历时经过的边。

### 数据范围

- $2\le N\le M\le 10^6$。



### 输入格式

一行两个数 $N,M$。

### 输出格式

一行一个数，表示答案。

### 样例解释 $\textbf 1$

只有 $a=(2,2)$ 合法。


**Translated by @nr0728.**

```input1
2 2
```

```output1
1
```

```input2
3 4
```

```output2
9
```

```input3
10 20
```

```output3
186225754
```

```input4
100000 1000000
```

```output4
191021899
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ M\ \leq\ 10^6 $
- 入力される値はすべて整数である

### Sample Explanation 1

あり得るのは $ a=(2,2) $ のみです． $ G $ は多重辺を持ってもよいことに注意してください．

