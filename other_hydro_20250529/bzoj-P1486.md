## 题目描述

考虑带权的有向图 $G=(V,E)$ 以及 $w:E \rightarrow R$，每条边 $e=(i,j)(i\neq j,i\in V,j\in V)$ 的权值定义为 $w_{i,j}$，令 $n=|V|$。$c=(c_1,c_2,\cdots,c_k)(c_i\in V)$ 是 $G$ 中的一个圈当且仅当 $(c_i,c_{i+1})(1\le i<k)$ 和 $(c_k,c_1)$ 都在 $E$ 中，这时称 $k$ 为圈 $c$ 的长度同时令 $c_{k+1}=c_1$，并定义圈 $c=(c_1,c_2,\cdots,c_k)$ 的平均值为 $\mu(c)=\sum\limits_{i=1}^{k} w_{c_i,c_{i+1}}/k$，即 $c$ 上所有边的权值的平均值。令 $\mu'(c)=\min(\mu(c))$ 为 $G$ 中所有圈 $c$ 的平均值的最小值。现在的目标是：在给定了一个图 $G=(V,E)$ 以及 $w:E \rightarrow R$ 之后，请求出 $G$ 中所有圈 $c$ 的平均值的最小值 $\mu'(c)=\min(\mu(c))$

## 输入格式

第一行 $2$ 个正整数，分别为 $n$ 和 $m$，并用一个空格隔开，只用 $n=|V|,m=|E|$ 分别表示图中有 $n$ 个点 $m$ 条边。

接下来 $m$ 行，每行 $3$ 个数 $i,j,w_{i,j}$，表示有一条边 $(i,j)$ 且该边的权值为 $w_{i,j}$。

输入数据保证图 $G=(V,E)$ 连通，存在圈且有一个点能到达其他所有点。

## 输出格式

请输出一个实数 $\mu'(c)=\min(\mu(c))$，要求输出到小数点后 $8$ 位。

```input1
4 5
1 2 5
2 3 5
3 1 5
2 4 3
4 1 3
```

```output1
3.66666667
```
