## ��Ŀ����
The cross-country skiing course at the winter Moolympics is described by an M x N grid of elevations (1 <= M,N <= 500), each elevation being in the range 0 .. 1,000,000,000.

Some of the cells in this grid are designated as starting points for the course.  The organizers of the Moolympics want to assign a difficulty rating to each starting point.  The difficulty level of a starting point P should be the minimum possible value of D such that a cow can successfully reach at least T total cells of the grid (1 <= T <= MN), if she starts at P and can only move from cell to adjacent cell if the absolute difference in elevation between the cells is at most D.  Two cells are adjacent if one is directly north, south, east, or west of the other.

Please help the organizers compute the difficulty rating for each starting point.

��ѩ����һ��M\*N(1 <= M,N <= 500)�����־����ʾ���θ߶ȣ�ÿ�����ֱ�ʾһ����Χ��0 .. 1,000,000,000�ĸ߶ȡ���Щ���ӱ�ָ��Ϊ��㣬��֯�������Щ������Ѷ�������


������P����һ���Ѷȼ���ΪD����㣬��D��������������������һ����Сֵ��


��1����һ������ֻ�ܻ������ڵĸ��ӣ�


��2�����������ӵĺ��β����D��


��3�������ܹ�����T��1 <= T <= M\*N�������ӣ�������㱾����


## �����ʽ
\* Line 1: The integers M, N, and T.

\* Lines 2..1+M: Each of these M lines contains N integer elevations.

\* Lines 2+M..1+2M: Each of these M lines contains N values that are either 0 or 1, with 1 indicating a cell that is a starting point.


## �����ʽ
\* Line 1: The sum of difficulty ratings of all starting points (note that this may not fit into a 32-bit integer, even though individual difficulty ratings will).


```input1
3 5 10 
20 21 18 99 5 
19 22 20 16 17 
18 17 40 60 80 
1 0 0 0 0 
0 0 0 0 0 
0 0 0 0 1 

```

```output1
24 

```

## ��ʾ
The ski course is described by a 3 x 5 grid of elevations.  The upper-left and lower-right cells are designated as starting points.  From each starting point, we must be able to reach at least 10 cells.


The difficulty rating of the upper-left starting point is 4, and for the lower-right it is 20.


