## ��Ŀ����
It's Bessie's birthday and time for party games! Bessie has instructed the N (1 <= N <= 100,000) cows conveniently numbered 1..N to sit in a circle (so that cow i [except at the ends] sits next to cows i-1 and i+1; cow N sits next to cow 1). Meanwhile, Farmer John fills a barrel with one billion slips of paper, each containing some integer in the range 1..1,000,000.

Each cow i then draws a number A\_i (1 <= A\_i <= 1,000,000) (which is not necessarily unique, of course) from the giant barrel.  Taking turns, each cow i then takes a walk around the circle and pats the heads of all other cows j such that her number A\_i is exactly

divisible by cow j's number A\_j; she then sits again back in her original position.

The cows would like you to help them determine, for each cow, the number of other cows she should pat.



## �����ʽ
\* Line 1: A single integer: N

\* Lines 2..N+1: Line i+1 contains a single integer: A\_i


## �����ʽ
\* Lines 1..N: On line i, print a single integer that is the number of other cows patted by cow i.


## ��Ŀ����
�����Ǳ�������գ�Ϊ����ף�Լ������գ�������������һ����Ϸ��

������ $N$ ($1\leq N\leq 10^5$) ͷ��ţ����һ��Ȧ������ $1$ ���� $N$ ����ţ�⣬$i$ ����ţ�� $i-1$ �ź� $i+1$ ����ţ���ڡ�$N$ ����ţ�� $1$ ����ţ���ڡ�ũ��Լ���úܶ�ֽ��װ����һ��Ͱ��ÿһ�Ű�����һ����һ���Ƕ�һ�޶��� $1$ �� $10^6$ �����֡�

����ÿһͷ��ţ $i$ ��Ͱ��ȡ��һ��ֽ�� $A_i$��ÿͷ��ţ��������һȦ��ͬʱ�Ĵ����������������������Լ�ֽ���ϵ����ֵ�ţ��ͷ��Ȼ�����ص�ԭ����λ�á�ţ��ϣ�����������ȷ����ÿһͷ��ţ��Ҫ�Ĵ��ţ��������


```input1
5 
2 
1 
2 
3 
4 

```

```output1
2 
0 
2 
1 
3 

```

## ��ʾ
The 5 cows are given the numbers 2, 1, 2, 3, and 4, respectively.


The first cow pats the second and third cows; the second cows pats no cows; etc.


