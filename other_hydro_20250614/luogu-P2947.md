## ��Ŀ����
Farmer John's N (1 <= N <= 100,000) cows, conveniently numbered 1..N, are once again standing in a row. Cow i has height H\_i (1 <= H\_i <= 1,000,000).

Each cow is looking to her left toward those with higher index numbers. We say that cow i 'looks up' to cow j if i < j and H\_i < H\_j. For each cow i, FJ would like to know the index of the first cow in line looked up to by cow i.

Note: about 50% of the test data will have N <= 1,000. 

Լ���� $N(1\le N\le10^5)$ ͷ��ţվ��һ�ţ���ţ $i$ ������� $H_i(1\le H_i\le10^6)$�����ڣ�ÿֻ��ţ�������ҿ��롣������ţ $i$�������ţ $j$ ���� $i<j$ �� $H_i<H_j$�����ǿ���˵��ţ $i$ ����������ţ $j$�� ���ÿֻ��ţ�����������������

Input

## �����ʽ
1. \* Line 1: A single integer: N

\* Lines 2..N+1: Line i+1 contains the single integer: H\_i

�� $1$ ������ $N$��֮��ÿ������һ����� $H_i$��


## �����ʽ
\* Lines 1..N: Line i contains a single integer representing the smallest index of a cow up to which cow i looks. If no such cow exists, print 0.

�� $N$ �У���˳��ÿ�����һֻ��ţ����������������û������������� $0$��


```input1
6 
3 
2 
6 
1 
1 
2 

```

```output1
3 
3 
0 
6 
6 
0 

```

## ��ʾ
FJ has six cows of heights 3, 2, 6, 1, 1, and 2.


Cows 1 and 2 both look up to cow 3; cows 4 and 5 both look up to cow 6; and cows 3 and 6 do not look up to any cow.

������˵����$6$ ͷ��ţ����߷ֱ�Ϊ 3,2,6,1,1,2��

�����˵������ţ #1,#2 ������ţ #3����ţ #4,#5 ������ţ #6����ţ #3 �� #6 û����������

�����ݹ�ģ��

���� $20\%$ �����ݣ�$1\le N\le10$��

���� $50\%$ �����ݣ�$1\le N\le10^3$��

���� $100\%$ �����ݣ�$1\le N\le10^5,1\le H_i\le10^6$��


