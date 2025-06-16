## 题目描述
You are given a tree consisting of $n$ vertices. Each vertex $i$ of this tree has a value $w_i$ assigned to it.

Now the vertex $u$ will be broken. Once it's broken, vertex $u$ and all edges with one end at vertex $u$ will be removed from the tree.

To make the tree connected, you can do the following operation any number of times(possibly zero) in any order:

- First choose two vertices $u$ and $v$ from the tree;
- Then pay $w_u+w_v$ coins, and add an edge between vertices $u$ and $v$;
- At last, replace $w_u+1$ with $w_u$, replace $w_v+1$ with $w_v$.

Your task is to calculate the minimum number of coins to be paid.

But you don't know which vertex $u$ is, so you need to find the answer for each $1\le u\le n$. Please answer all the queries independently.

## 输入格式
The first line contains a single integer $n(2\le n\le 10^6)$ --- the number of vertices in this tree.

The next line contains $n$ numbers, the $i$ -th number is $w_i(1\le w_i\le n)$.

The next $n-1$ lines contain a description of the tree's edges. The $i$ -th of these lines contains two integers $u_i$ and $v_i(1\le u_i,v_i\le n) $ --- the numbers of vertices connected by the $i$ -th edge.

It is guaranteed that the given edges form a tree.

## 输出格式
Print $n$ integers, the $i$ -th integer is the answer when $u=i$.

```input1
6
1 1 1 1 1 1
1 2
1 3
1 4
2 5
2 6
```

```output1
4 4 0 0 0 0
```

```input2
4
1 2 3 4
1 2
1 3
1 4
```

```output2
12 0 0 0
```

```input3
7
1 2 3 4 5 6 7
1 2
1 3
2 4
2 5
3 6
3 7
```

```output3
5 12 16 0 0 0 0
```

## 提示
给定一个有 $n$ 个点组成的树，每个点有一个权值 $w_i$。  
点 $u$ 和相邻的边被删除。  
你可以进行以下操作任意次数（可以为 $0$）,让树重新成为连通图：
1. 选择两个点 $u$、$v$；
2. 花费 $w_u + w_v$ 的代价连接一条边 $(u,v)$；
3. $w_u \leftarrow w_u+1,w_v \leftarrow w_v+1$。

对于每个 $u$ 计算最小代价。

