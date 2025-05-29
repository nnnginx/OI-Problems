## 题目背景
![](https://cdn.luogu.com.cn/upload/image_hosting/4ifpqjie.png)

## 题目描述
星野爱给了你一张无向图 $G$，设 $R(i)$ 为所有与 $i$ 相连的边的另一个端点构成的可重集合，可能有重边，没有自环。

每个节点有权值 $w_i$，初始时都为 $0$，需要维护两种操作。

- `1,l,r,v`，对于 $i\in [l,r]$，$j\in R(i)$，令 $w_j=w_j+v$
- `2,l,r`，计算 $\sum_{i\in[l,r]}\sum_{j\in R(i)}w_j$。

输出的值请对 $2^{64}$ 取模。



## 输入格式

第一行三个整数 $n,m,q$。

接下来 $m$ 行，每行两个整数 $u,v$ 代表一条边。

接下来 $q$ 行，每行三个或四个整数代表一个操作。

## 输出格式
对于操作二，每行输出一个整数表示计算的结果。

```input1
6 6 5
2 6
6 1
5 3
1 5
3 1
2 4
1 1 6 1
1 2 4 3
1 3 4 3
2 3 6
2 1 2
```

```output1
53
24
```

## 提示
Idea：Larunatrecy，Solution：Larunatrecy，Code：Larunatrecy，Data：Larunatrecy

对于 $20\%$ 的数据，$1\leq n,m,q\leq 5000$。

对于 $40\%$ 的数据，$1\leq n,m,q\leq 5\times 10^4$。

对于另外 $10\%$ 的数据，$l=r$ 恒成立。

对于 $100\%$ 的数据，$1\leq n,m,q\leq 2\times 10^5,0\leq v\leq 10^9$。

