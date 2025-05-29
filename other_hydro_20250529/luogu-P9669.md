## ��Ŀ����
Prof. Pang has a rooted tree that is rooted at vertex $1$ and has $n$ nodes. These $n$ nodes are numbered from $1$ to $n$.

Now he wants to start the depth-first search at the root. He wonders for each node $v$, how many ways it can appear in the $j$-th position of $\textbf{depth-first search order}$. The depth-first search order is the order of nodes visited during the depth-first search. A node appears in the $j$-th ($1\le j\le n$) position in this order means it is visited after $j-1$ other nodes. Because sons of a node can be iterated in arbitrary order, multiple possible depth-first orders exist. 

Prof. Pang wants to know for each node $v$, how many different $\textbf{depth-first search order}$s such that $v$ appears in the $j$-th position. For each $v, j~(1 \le v, j \le n)$, compute the answer. Because the answer can be very large, output it modulo $998244353$.

Following is a pseudo-code for the depth-first search on a rooted tree. After calling $\textbf{main}$(), $\texttt{dfs\_order}$ is the depth-first search order.

![](https://cdn.luogu.com.cn/upload/image_hosting/l3gjstn0.png)

## �����ʽ
The first line contains one integer $n~(1\le n \le 500)$, the number of vertices in the tree.

Each of the next $n-1$ lines describes an edge of the tree. Edge $i$ is denoted by two integers $u_i$ and $v_i$, the labels of vertices it connects $(1\le u_i,v_i\le n, u_i\neq v_i)$.

It is guaranteed that the given edges form a tree.

## �����ʽ
For each vertex $v$ from $1$ to $n$, output one line containing $n$ integers modulo $998244353$. The $j$-th integer in the $v$-th line should be the number of different depth-first search orders such that $v$ appears in the $j$-th position.

## ��Ŀ����
### ��Ŀ����

P��һ���������ڵ���$1$���ܹ���$n$���ڵ㣬��$1$��$n$��š�

����Ӹ��ڵ㿪ʼ���������������������֪������ÿ���ڵ�$v$����������������У��������ڵ�$j$��λ�õķ�ʽ�ж����֡��������������˳���������������з��ʽڵ��˳�򡣽ڵ�����ڵ�$j��1 \le j \le n $����λ�ñ�ʾ���ڷ�����$j - 1$�������ڵ�֮��ű����ʡ���Ϊ�ڵ���ӽڵ����������˳����ʣ������ж��ֿ��ܵ������������˳��

P��֪������ÿ���ڵ�$v$���ж����ֲ�ͬ�������������˳��ʹ��$v$�����ڵ�$j$��λ�á�����ÿ��$v$��$j��i \le v,j \le n��$������𰸡��𰸿��ܴܺ��������ʱҪȡģ$998244353$���������������������α���룬���ڴ��������ڵ���$main()$������ dfs_order��������������������˳��



------------
#### �㷨 $1$ �������������ʵ��
```
1. ���� DFS(�ڵ� x)

2.	��x��ӵ�dfs_order��ĩβ

3.	����x��ÿ���ӽڵ�y do               ���ӽڵ����������˳�������

4.		DFS(y)

5.	����ѭ��

6. ��������

7. ���� MAIN()

8.	��dfs_order��Ϊȫ�ֱ���

9.	dfs_order �� ���б�

10.	DFS(1)

11. ��������
```
------------

### �����ʽ

��һ�а���һ������$n��1\le n\le 500��$����ʾ���еĽڵ�������

��������n-1�����������ıߡ���i�а�����������$u_i$��$v_i$����ʾ���ӵ������ڵ�ı�ǩ$��1\le u_i,v_i\le n,u_i\not=v_i��$��

��֤�����ı߹���һ������

### �����ʽ

����ÿ����$1$��$n$�Ľڵ�$v$�����һ�У�����$n$��������ȡģ$998244353$���ڵ�$v$���У���$j$��������ʾ��ͬ�������������˳���У��ڵ�$v$�����ڵ�$j$��λ�õ�������

 	������@ayf2192538031�ṩ

```input1
5
1 2
1 3
3 4
3 5
```

```output1
4 0 0 0 0
0 2 0 0 2
0 2 2 0 0
0 0 1 2 1
0 0 1 2 1
```

