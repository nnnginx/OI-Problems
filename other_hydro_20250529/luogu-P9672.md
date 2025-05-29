## ��Ŀ����
You are given a simple polygon in the first quadrant of the Cartesian plane. This means that the coordinate $(x, y)$ of any point in the polygon satisfies $x> 0$ and $y> 0$. 

Consider all grid points in the polygon. Order them in increasing order of \textbf{slopes}. Output the $k$-th grid point in this order. 

A grid point is a point $(x, y)$ such that $x$ and $y$ are integers. A point on the boundary of a polygon is considered to be in the polygon. The slope of point $(x, y)$ is $y/x$. If two points have the same slope, they are ordered lexicographically first by $x$, then by $y$. In other words, a point $(x_1, y_1)$ is lexicographically less than $(x_2, y_2)$ if $(x_1<x_2)\vee (x_1=x_2 \wedge y_1<y_2)$. 

## �����ʽ
The first line contains one integer $T~(1\le T \le 500)$, the number of test cases.

For each test case, the first line contains two integers $n, k~(n\ge 3, 1\le k)$. Each of the next $n$ lines describes a vertex of the polygon. Each vertex is denoted by two integers $x, y~(1\le x, y\le 10^9)$, representing its coordinate $(x, y)$. The vertices are given in counterclockwise order.

It is guaranteed that the polygon is simple, i.e.~ the vertices are distinct, two edges may overlap only when they are consecutive on the boundary, and the overlap contains exactly $1$ point. It is guaranteed that $k$ is no more than the number of grid points in the polygon.

It is guaranteed that the sum of $n$ over all test cases is no more than $2000$.

## �����ʽ
For each test case, output two integers $x, y$ in one line representing the coordinate $(x, y)$ of the $k$-th grid point.

## ��Ŀ����
## ��Ŀ����



�ڵѿ���ƽ��ĵ�һ�������У�����õ�һ���򵥵Ķ���Ρ�����ζ�Ŷ�������κε������$��x��y��$����$x>0$��$y>0$��



���Ƕ�����е���������㡣��\textbf��б�ʣ��ĵ���˳�����С�����˳�������$k$������㡣



�������һ����$��x��y��$��ʹ��$x$��$y$������������α߽��ϵ�һ���㱻��Ϊ�ڶ�����С���$��x��y��$��б��Ϊ$y/x$����������������ͬ��б�ʣ����������Ȱ��ֵ�˳������$x$��Ȼ��$y$�����仰˵�����$��x_1<x_2��\vee��x_1=x_2\wedge y_1<y_2��$�����$��x_1��y_1��$���ֵ���С��$��x_2��y_2����



## �����ʽ



��һ�а���һ������$T~��1\le T\le 500��$��������������������



����ÿ��������������һ�а�����������$n��k~��n\ge 3��1\le k��$����������ÿһ��$n$�߶������˶���ε�һ�����㡣ÿ����������������$x��y~��1\le x��y\le 10^9��$��ʾ����ʾ������$��x��y��$�����㰴��ʱ��˳�����С�



��֤������Ǽ򵥵ģ��������ǲ�ͬ�ģ�������ֻ���ڱ߽�������ʱ�����ص��������ص�ǡ�ð���$1$�㡣���Ա�֤$k$������������е����������



��֤���в����������ܽ�����2000��Ԫ��



## �����ʽ



����ÿ��������������һ���������������$x��y$����ʾ��$k$������������$��x��y��$��



## �����������



### ���� #1



```
4
3 3
1 1
3 1
3 3
4 5000000000000000
1 1
1000000000 1
1000000000 1000000000
100000000
9 22
9 6
6 7
9 7
10 10
6 9
3 9
1 6
1 5
7 3
5 22447972861454999
270353376 593874603
230208698 598303091
237630296 255016434
782669452 568066304
654623868 958264153
```



### ��� #1



```
3 2
500000000 500000000
7 8
730715389 644702744
```

```input1
4
3 3
1 1
3 1
3 3
4 500000000000000000
1 1
1000000000 1
1000000000 1000000000
1 1000000000
9 22
9 6
6 7
9 7
10 10
6 9
3 9
1 6
1 5
7 3
5 22447972861454999
270353376 593874603
230208698 598303091
237630296 255016434
782669452 568066304
654623868 958264153
```

```output1
3 2
500000000 500000000
7 8
730715389 644702744
```

