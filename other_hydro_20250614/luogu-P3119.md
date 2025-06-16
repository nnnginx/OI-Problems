## ��Ŀ����
In an effort to better manage the grazing patterns of his cows, Farmer John has installed one-way cow paths all over his farm. The farm consists of N fields, conveniently numbered 1..N, with each one-way cow path connecting a pair of fields. For example, if a path connects from field X to field Y, then cows are allowed to travel from X to Y but not from Y to X.

Bessie the cow, as we all know, enjoys eating grass from as many fields as possible. She always starts in field 1 at the beginning of the day and visits a sequence of fields, returning to field 1 at the end of the day. She tries to maximize the number of distinct fields along her route, since she gets to eat the grass in each one (if she visits a field multiple times, she only eats the grass there once).

As one might imagine, Bessie is not particularly happy about the one-way restriction on FJ's paths, since this will likely reduce the number of distinct fields she can possibly visit along her daily route.  She wonders how much grass she will be able to eat if she breaks the rules and follows up to one path in the wrong direction. Please compute the maximum number of distinct fields she can visit along a route starting and ending at field 1, where she can follow up to one path along the route in the wrong direction.  Bessie can only travel backwards at most once in her journey.  In particular, she cannot even take the same path backwards twice.

## �����ʽ
The first line of input contains N and M, giving the number of fields and the number of one-way paths (1 <= N, M <= 100,000). 

The following M lines each describe a one-way cow path.  Each line contains two distinct field numbers X and Y, corresponding to a cow path from X to Y.  The same cow path will never appear more than once.

## �����ʽ
A single line indicating the maximum number of distinct fields Bessie can visit along a route starting and ending at field 1, given that she can follow at most one path along this route in the wrong direction.

## ��Ŀ����
### ��Ŀ����

Ϊ�˸��õع���ţȺ�ķ���·�ߣ�Farmer John ������ũ���а�װ�����ɵ���ţ����ũ���� $N$ ��ݳ���ɣ����Ϊ $1$ �� $N$��ÿ������ţ������һ�Բݳ������磬������һ���Ӳݳ� $X$ �� $Y$ ��·������ţ���Դ� $X$ ǰ�� $Y$�������ܴ� $Y$ ���� $X$��

������֪��Bessie ϲ�������ܶ��Ʒ����ͬ�ݳ������ݡ���ÿ��Ӳݳ� $1$ ����������һϵ�вݳ��󷵻زݳ� $1$������ͼ�����;�����Ĳ�ͬ�ݳ��������ظ����ʵĲݳ�ֻ��һ�Σ���

���ڵ���·�������ƣ�Bessie ������������ÿ��·���п��Է��ʵĲݳ�����������֪�������Υ��������·�����������ͨ��ĳ����·һ�Σ������Ʒ�����ٲݳ������ݡ���������Ӳݳ� $1$ ���������ص�����£�����ܷ��ʵĲ�ͬ�ݳ�������ע�� Bessie �������ó������ֻ������ͨ��һ����·����ͬһ��·�������������Ρ�

### �����ʽ

��һ�а����������� $N$ �� $M$����ʾ�ݳ������͵���ţ��������$1 \leq N, M \leq 100,000$����

������ $M$ ��ÿ������һ������ţ��������������ͬ������ $X$ �� $Y$����ʾ�� $X$ �� $Y$ �ĵ���·������֤ÿ��·�������ظ����֡�

### �����ʽ

���һ�У���ʾ Bessie ���������ͨ��һ����·������£��Ӳݳ� $1$ ����������ʱ�ܷ��ʵ����ͬ�ݳ�������

### ˵��/��ʾ

**����������**

��������������� ASCII ͼʾ��

```
v---3-->6
7   | \ |
^\  v  \|
| \ 1   |
|   |   v
|   v   5
4<--2---^
```

Bessie ����ͨ������·�� $5\to 3$ ���ʲݳ� $1, 2, 4, 7, 2, 5, 3, 1$������ݳ� $3$ �������ٴ���������·�����޷�ǰ�� $6$��

```input1
7 10 
1 2 
3 1 
2 5 
2 4 
3 7 
3 5 
3 6 
6 5 
7 2 
4 7 


```

```output1
6 

```

## ��ʾ
SOLUTION NOTES:

Here is an ASCII drawing of the sample input:

```cpp
v---3-->6
7   | \ |
^\  v  \|
| \ 1   |
|   |   v
|   v   5
4<--2---^
```

Bessie can visit pastures 1, 2, 4, 7, 2, 5, 3, 1 by traveling backwards on the path between 5 and 3.  When she arrives at 3 she cannot reach 6 without following another backwards path.

