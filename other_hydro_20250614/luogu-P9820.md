## ��Ŀ����
A mine-sweeper map $X$ can be expressed as an $n\times m$ grid. Each cell of the grid is either a mine cell or a non-mine cell. A mine cell has no number on it. Each non-mine cell has a number representing the number of mine cells around it. (A cell is around another cell if they share at least one common point. Thus, every cell that is not on the boundary has $8$ cells around it.) The following is a $16\times 30$ mine-sweeper map where a flagged cell denotes a mine cell and a blank cell denotes a non-mine cell with number 0.

![](https://cdn.luogu.com.cn/upload/image_hosting/5bykwzuy.png)

Given two mine-sweeper maps $A, B$ of size $n\times m$, you should modify at most $\left\lfloor\frac{nm}{2}\right\rfloor$ (i.e. the largest nonnegative integer that is less than or equal to $\frac{nm}{2}$) cells in $B$ (from a non-mine cell to a mine cell or vice versa) such that the sum of numbers in the non-mine cells in $A$ and the sum of numbers in the non-mine cells in $B$ are the same. (If a map has no non-mine cell, the sum is considered as $0$.)

If multiple solutions exist, print any of them. If no solution exists, print ``-1`` in one line.

## �����ʽ
The first line contains two integers $n, m\,(1\le n,m \le 1000)$, denoting the size of given mine-sweeper maps.

The $i$-th line of the following $n$ lines contains a length-$m$ string consisting of  ``.`` and ``X`` denoting the $i$-th row of the mine-sweeper map $A$. A ``.`` denotes for a non-mine cell and an ``X`` denotes for a mine cell.

The $i$-th line of the following $n$ lines contains a length-$m$ string consisting of  ``.`` and ``X`` denoting the $i$-th row of the mine-sweeper map $B$. A ``.`` denotes for a non-mine cell and an ``X`` denotes for a mine cell.

## �����ʽ
If no solution exists, print ``-1`` in one line.

Otherwise, print $n$ lines denoting the modified mine-sweeper map $B$. The $i$-th line should contain a length-$m$ string consisting of  ``.`` and ``X`` denoting the $i$-th row of the modified map $B$. A ``.`` denotes for a non-mine cell and an ``X`` denotes for a mine cell.

Please notice that you need not print the numbers on non-mine cells since these numbers can be determined by the output mine-sweeper map.

## ��Ŀ����
һ��ɨ�׵�ͼ $X$ ���Ա���Ϊһ�� $n \times m$ ������ÿ������Ҫô�ǵ��׸�Ҫô���ǵ��׸񡣵��׸���û�����֣���ÿ���ǵ��׸��϶���һ�����֣�������Χ���� $8$ �������е��׸����Ŀ����ͼ��һ�� $16\times 30$ ��ɨ�׵�ͼ�����׸���С�����ʾ��һ���հ׵ĸ��Ӵ���һ������Ϊ $0$ �ķǵ��׸�

![](https://cdn.luogu.com.cn/upload/image_hosting/5bykwzuy.png)


�������ųߴ��Ϊ $n\times m$ ��ɨ�׵�ͼ $A,B$��ÿ���޸Ŀ��Խ�һ�����׸��Ϊ�ǵ��׸񣬻��߽�һ���ǵ��׸��Ϊ���׸�������޸���� $\lfloor \dfrac{nm}{2} \rfloor$ ����ͼ $B$ �еĸ��ӣ������һ�ַ�����ʹ�� $A,B$ �зǵ��׸�������֮����ͬ�����޽⣬��� $-1$��

```input1
2 4
X..X
X.X.
X.X.
.X..
```

```output1
X.XX
.X..
```

## ��ʾ
We modify one cell in $B$. Then the sums of the numbers on non-mine cells in $A$ and $B$ both equal $10$.

