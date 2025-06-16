## ��Ŀ����
Farmer John has purchased N (5 <= N <= 250) fence posts in order to build a very nice-looking fence. Everyone knows the best fences are convex polygons where fence posts form vertices of a polygon. The pasture is represented as a rectilinear grid; fencepost i is at integer coordinates (x\_i, y\_i) (1 <= x\_i <= 1,000; 1 <= y\_i <= 1000).

Given the locations of N fence posts (which, intriguingly, feature no set of three points which are collinear), what is the largest number of fence posts FJ can use to create a fence that is convex?

For test cases worth 45% of the points for this problem, N <= 65.

Time limit: 1.2 seconds

POINTS: 400

Farmer John��ũ������N��5<=N<=250�������׮��ÿ�����ж�һ�޶�������(xi,yi)��1<=xi,yi<=1000��������ѡ����������׮����������Χ�������Χ��Ҫ���ۣ����Ա�����͹����εġ����������ѡ���ٸ��أ�

���е����׮�в��������㹲�ߡ�


## �����ʽ
\* Line 1: A single integer: N

\* Lines 2..N+1: Line i+1 describes fence post i's location with two space-separated integers: x\_i and y\_i


## �����ʽ
\* Line 1: A single integer, the maximum possible number of fence posts that form a convex polygon.


```input1
6 
5 5 
2 3 
3 2 
1 5 
5 1 
1 1 

```

```output1
5 

```

## ��ʾ
A square with two points inside.


The largest convex polygon is the pentagon (2,3), (3,2), (5,1), (5,5), (1,5).


