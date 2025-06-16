## ��Ŀ����
One of Farmer John's fields is particularly hilly, and he wants to purchase a new tractor to drive around on it.  The field is described by an N x N grid of non-negative integer elevations (1 <= N <= 500).  A tractor capable of moving from one grid cell to an adjacent cell (one step north, east, south, or west) of height difference D costs exactly D units of money.

FJ would like to pay enough for his tractor so that, starting from some grid cell in his field, he can successfully drive the tractor around to visit at least half the grid cells in the field (if the number of total cells in the field is odd, he wants to visit at least half the cells rounded up).  Please help him compute the minimum cost necessary for buying a tractor capable of this task.


## �����ʽ
\* Line 1: The value of N.

\* Lines 2..1+N: Each line contains N space-separated non-negative integers (each at most 1 million) specifying a row of FJ's field.






## �����ʽ
\* Line 1: The minimum cost of a tractor that is capable of driving around at least half of FJ's field.




## ��Ŀ����
��Ŀ����

FJ�п�ũ��̫����ˣ���Ҫ��һ��������������������Ѳ�ӡ����ũ����N x N�����ӵķǸ�������ʾ�߶�(1<=N<=500)���������ӵ�ǰ�����ߵ����ڸ��ӣ������ϡ��������ĸ����򣩵Ĵ���Ϊ�߶Ȳ�D����FJʻ�����������ӵ�����������ҲҪֵD��Ǯ��

FJԸ�⻨�㹻��Ǯ��һ���µ�������ʹ����������С�ĸ߶Ȳ��߱����и��ӵ�һ��(���������������������ôһ���ֵΪ���������ֵ)����ΪFJ�������������ҵ��������̼�������С��Ҫ������Ǯ�򵽷�����ЩҪ�����������

���������ʽ

�����ʽ��

��һ��Ϊһ������N

��2��N+1��ÿ�а���N���Ǹ�������������1,000,000������ʾ��ǰ���ӵĸ߶ȡ�

�����ʽ��

��һ�У���ʾFJ��������Ҫ������С��Ǯ��

```input1
5 
0 0 0 3 3 
0 0 0 0 3 
0 9 9 3 3 
9 9 9 3 3 
9 9 9 9 3 

```

```output1
3 

```

