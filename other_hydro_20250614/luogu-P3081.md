## ��Ŀ����
There are N hills (1 <= N <= 100,000). Each hill takes the form of a line segment from (x1, y1) to (x2, y2) where x1 < x2 and y1 < y2. None of these segments intersect or touch, even at their endpoints, and furthermore, the first hill satisfies (x1, y1) = (0,0).

Bessie the cow starts at (0,0) on the first hill. Whenever Bessie is on a hill, she climbs up until she reaches the end. Then she jumps off the edge. If she lands on another hill, she continues walking on that hill; otherwise, she falls very far until she lands safely on a cushion of pillows at y = -infinity.  Each hill (x1, y1) -> (x2, y2) should be regarded as containing the point (x1, y1) but not containing the point (x2, y2), so that Bessie will land on the hill if she falls on it from above at a position with x = x1, but she will not land on the hill if she falls on it from above at x = x2.

Please count the total number of hills that Bessie touches at some point during her walk.

�� $N(1 \le N \le 10 ^ 5)$��Сɽ��ÿ��ɽ��ռ��������ֱ�� $(x1, y1)$ �� $(x2, y2)$ ����ʾ��$x1 < x2$ ���� $y1 < y2$����Ҳ����˵��Щɽ�õѿ�������ϵ����߶�����ʾ����Щ���ڱ�ʾСɽ���߶ζ�û���κν��㣬��һ��ɽ��һ��λ�� $(x1, y1) = (0,0)$��


������ $(0,0)$ ��ʼ�ڵ�һ��ɽ��������һ����������һ��ɽ������һֱ�ߵ���ɽ���յ㣬��ʱ������ӱ�Ե����������������䵽��һ��ɽ�ϣ�����������µ�ɽ�������������������� $y$ �᷽�����䣬����������ܽ��䵽һ��ɽ�ϣ�����һֱ���䣬ֱ������ $y$ ��ĸ������λ�ã�$y = -\infin$����


ÿ�����߶α�ʾ��ɽ $(x1, y1) \to (x2, y2)$ ���� $(x1, y1)$ ����㣬�������� $(x2, y2)$�������������ܹ��ڶ�����ɽ�������ˡ�


## �����ʽ
\* Line 1: The number of hills, N.

\* Lines 2..1+N: Line i+1 contains four integers (x1,y1,x2,y2)

describing hill i.  Each integer is in the range

0..1,000,000,000.


## �����ʽ
\* Line 1: The number of hills Bessie touches on her journey.


```input1
4 
0 0 5 6 
1 0 2 1 
7 2 8 5 
3 0 7 7 

```

```output1
3 

```

## ��ʾ
There are four hills.  The first hill runs from (0,0) to (5,6), and so on.


Bessie walks on hills #1, #4, and finally #3.


