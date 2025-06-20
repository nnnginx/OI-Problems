# AT_abc251_f 两颗生成树

## 题目描述

给定一个有 $N$ 个顶点和 $M$ 条边的无向图 $G$。$G$ 是简单图（即无自环和无重边）且连通的。

对于 $i = 1,2,\dots,M$，第 $i$ 条边是顶点 $u_i$ 和顶点 $v_i$ 和无向边边 $u_i\Leftrightarrow v_i$。

图 $G$ 的两棵全局树 $T_1$ 和 $T_2$，同时满足以下两个条件（$T_1$ 和 $T_2$ 可以相同）。

- $T_1$ 满足以下条件：
>  $T_1$ 是一棵以顶点 1 为根的有根树，对于原图 $G$ 上的两点 $u$ 和 $v$ 有 $u\Leftrightarrow v$，若这条边不是生成树中的树边，那么在生成树上这两点一定是祖先关系。
- $T_2$ 满足以下条件：
> $T_2$ 是一棵以顶点 1 为根的有根树，对于原图 $G$ 上的两点 $u$ 和 $v$ 有 $u\Leftrightarrow v$，若这条边不是生成树中的树边，那么在生成树上这两点一定不是祖先关系。

## 输入格式

第一行输入两个正整数 $N$ 和 $M$。

第 $2$ 行到第 $M+1$ 行每行输入两个整数，表示在原图 $G$ 上有这条无向边。

## 输出格式

对于 $T_1$，输出从第 $1$ 行到第 $N-1$ 行，表示在满足 $T_1$ 生成条件下任意一棵生成树的所有边。

对于 $T_2$，输出从第 $2$ 行到第 $2N-2$ 行，表示在满足 $T_2$ 生成条件下任意一棵生成树的所有边。

注意：输出边的两个顶点顺序以及输出边的顺序都是任意的。

## 输入输出样例 #1

### 输入 #1

```
6 8
5 1
4 3
1 4
3 5
1 2
2 6
1 6
4 2
```

### 输出 #1

```
1 4
4 3
5 3
4 2
6 2
1 5
5 3
1 4
2 1
1 6
```

## 输入输出样例 #2

### 输入 #2

```
4 3
3 1
1 2
1 4
```

### 输出 #2

```
1 2
1 3
1 4
1 4
1 3
1 2
```

## 说明/提示

### 范围

- $2\le N\le 2\times 10^5$
- $N-1\le M \le \min \{ 2\times 10^5,\frac {N(N-1)}{2} \}$
- $1\le u_i,v_i\le N$
- 所有输入均为整数
- 给出的图简单且连通

### 样例解释 1
在上述输出示例中，$T_1$ 是具有 5 条边 $\{ \{ 1, 4 \}, \{ 4, 3 \}, \{ 5, 3 \}, \{ 4, 2 \}, \{ 6, 2 \} \}$ 的图 $G$ 的一棵生成树。

这棵 $T_1$ 满足问题描述中的条件。实际上，对于图 $G$ 中不在 $T_1$ 里的每条边：

-对于边 $\{ 5, 1 \}$，顶点 1 是顶点 5 的祖先；

-对于边 $\{ 1, 2 \}$，顶点 1 是顶点 2 的祖先； 

-对于边 $\{ 1, 6 \}$，顶点 1 是顶点 6 的祖先。 
 
$T_2$ 是具有 5 条边 $\{ \{ 1, 5 \}, \{ 5, 3 \}, \{ 1, 4 \}, \{ 2, 1 \}, \{ 1, 6 \} \}$ 的图 $G$ 的一棵生成树。
这棵 $T_2$ 满足问题描述中的条件。对于图 $G$ 中不在 $T_2$ 里的每条边： 

- 对于边 $\{ 4, 3 \}$，顶点 4 和顶点 3 不存在祖先——子孙关系；
- 对于边 $\{ 2, 6 \}$，顶点 2 和顶点 6 不存在祖先——子孙关系；
- 对于边 $\{ 4, 2 \}$，顶点 4 和顶点 2 不存在祖先——子孙关系。 
 
### 样例解释 2}
具有 3 条边 $\{ \{ 1, 2 \}, \{ 1, 3 \}, \{ 1, 4 \} \}$ 的树 $T$ 是图 $G$ 的唯一生成树。由于图 $G$ 中不存在不在这棵树 $T$ 里的边，显然，$T$ 同时满足 $T_1$ 和 $T_2$ 的条件。