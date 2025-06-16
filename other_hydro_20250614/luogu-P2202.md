## ��Ŀ����
Farmer John is planning to build N (2 <= N <= 50,000) square fenced-in pastures on his farm, each of size exactly K x K (1 <= K <= 1,000,000). Pasture i is centered at point (x\_i, y\_i) with integer coordinates in the range -1,000,000...1,000,000.  However, in his haste to complete his plans, FJ realizes that he may have accidentally placed two pastures in locations that overlap (by overlap, this means the two pastures share a positive area in common).  No two pastures share the exact same center point.

Given the locations of each of the planned square pastures, please help FJ compute the area shared by the two overlapping pastures.  Output zero if no two squares overlap, and -1 if overlap occurs between more than a single pair of pastures.

��һ��ֱ������ϵ�У���N���߳�ΪK�������Ρ�

����ÿһ�������ε����ģ����ж����е��������Ƿ����ص���

�������ݱ�֤ÿһ�������ε����Ĳ��غ�


## �����ʽ
\* ��1�� �������������� N , K

���У�2 <= N <= 50 000 ��1 <= K <= 1 000 000 ��K��֤��ż��

\*��2 .. i+1�У�ÿ������������xi��yi�������˵�i�������ε����ġ�

���У�xi��yi����[-1 000 000��1 000 000]��


## �����ʽ
ֻ���һ�У�

���û���������ص��������0�����������ֻ��һ���������ص�����������ص����������������Լ����ϵ��������غϣ����"-1";

ע�⣺������𰸺�һ��Ҫ�任�з���


```input1
4 6
0 0
8 4
-2 1
0 7
```

```output1
20
```

