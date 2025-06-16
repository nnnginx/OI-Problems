## ��Ŀ����


You are given a node-labeled rooted tree with n nodes. Define the query (x, k): Find the node whose label is k-th largest in the subtree of the node x. Assume no two nodes have the same labels.

## �����ʽ

The first line contains one integer n (1 <= n <= 10^5). The next line contains n integers li (0 <= li <= 109) which denotes the label of the i-th node. Each line of the following n - 1 lines contains two integers u, v. They denote there is an edge between node u and node v. Node 1 is the root of the tree. The next line contains one integer m (1 <= m <= 10^4) which denotes the number of the queries. Each line of the next m contains two integers x, k. (k <= the total node number in the subtree of x)



## �����ʽ


For each query (x, k), output the index of the node whose label is the k-th largest in the subtree of the node x.


## �ο�����


�����õ�һ������n���ڵ�Ľڵ��ǵĸ��������壺��ѯ��x��k�����ڽڵ�x���������ҵ���ǩ��k��Ľڵ㡣

**û�������ڵ������ͬ�ı�ǩ��**

�����ʽ
��һ�а���һ������$n$����һ�а���$n$������$li$������ʾ��$i$���ڵ�ı�ǩ����������$n-1$���е�ÿһ�ж�������������$u,v$�����Ǳ�ʾ�ڵ�$u$�ͽڵ�$v$֮�����һ���ߡ��ڵ�$1$�����ĸ�����һ�а���һ������$m$������ʾ��ѯ����������������$m$��ÿһ�а�����������$x,k$����$k$ <= x�������е��ܽڵ�����

## �������� 
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
## ������� 
```
5
4
5
5

```

## ���ݹ�ģ��Լ��

$1 \leq n \leq 10 ^ 5$

$0 \leq li \leq 109$

$1 \leq m \leq 10 ^ 4$

## ��ʾ

Amber��play with treeϵ�е���....


