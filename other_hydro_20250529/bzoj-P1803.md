## 题目描述


You are given a node-labeled rooted tree with n nodes. Define the query (x, k): Find the node whose label is k-th largest in the subtree of the node x. Assume no two nodes have the same labels.

## 输入格式

The first line contains one integer n (1 <= n <= 10^5). The next line contains n integers li (0 <= li <= 109) which denotes the label of the i-th node. Each line of the following n - 1 lines contains two integers u, v. They denote there is an edge between node u and node v. Node 1 is the root of the tree. The next line contains one integer m (1 <= m <= 10^4) which denotes the number of the queries. Each line of the next m contains two integers x, k. (k <= the total node number in the subtree of x)



## 输出格式


For each query (x, k), output the index of the node whose label is the k-th largest in the subtree of the node x.


## 参考翻译


您将得到一个带有n个节点的节点标记的根树。定义：查询（x，k）：在节点x的子树中找到标签第k大的节点。

**没有两个节点具有相同的标签。**

输入格式
第一行包含一个整数$n$。下一行包含$n$个整数$li$，它表示第$i$个节点的标签。接下来的$n-1$行中的每一行都包含两个整数$u,v$。它们表示节点$u$和节点$v$之间存在一条边。节点$1$是树的根。下一行包含一个整数$m$，它表示查询的数量。接下来的$m$的每一行包含两个整数$x,k$。（$k$ <= x的子树中的总节点数）

## 样例输入 
```
5
1 3 5 2 7
1 2
2 3
1 4
3 5
4
2 3
4 1
3 2
3 2

```
## 样例输出 
```
5
4
5
5

```

## 数据规模与约定

$1 \leq n \leq 10 ^ 5$

$0 \leq li \leq 109$

$1 \leq m \leq 10 ^ 4$

## 提示

Amber的play with tree系列的题....


