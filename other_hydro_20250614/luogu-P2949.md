## ��Ŀ����
Farmer John has so very many jobs to do! In order to run the farm efficiently, he must make money on the jobs he does, each one of which takes just one time unit.

His work day starts at time 0 and has 1,000,000,000 time units (!).  He currently can choose from any of N (1 <= N <= 100,000) jobs

conveniently numbered 1..N for work to do. It is possible but

extremely unlikely that he has time for all N jobs since he can only work on one job during any time unit and the deadlines tend to fall so that he can not perform all the tasks.

Job i has deadline D\_i (1 <= D\_i <= 1,000,000,000). If he finishes job i by then, he makes a profit of P\_i (1 <= P\_i <= 1,000,000,000).

What is the maximum total profit that FJ can earn from a given list of jobs and deadlines?  The answer might not fit into a 32-bit integer.




## �����ʽ
\* Line 1: A single integer: N

\* Lines 2..N+1: Line i+1 contains two space-separated integers: D\_i and P\_i


## �����ʽ
\* Line 1: A single number on a line by itself that is the maximum possible profit FJ can earn.


## ��Ŀ����
Լ����̫��Ĺ���Ҫ����Ϊ����ũ����Ч��ת�������뿿���Ĺ���׬Ǯ��ÿ�����һ����λʱ�䡣 ���Ĺ����մ� $0$ ʱ�̿�ʼ���� $10^9$ ����λʱ�䡣����һʱ�̣���������ѡ���� $1$ �� $N$ �� $N(1 \leq N \leq 10^5)$ ����е�����һ�������ɡ� ��Ϊ����ÿ����λʱ����ֻ����һ����������ÿ�������һ����ֹ���ڣ�������������ʱ���������N����������Ȼ�����п��ܡ� ���ڵ� $i$ ����������һ����ֹʱ�� $D_i(1 \leq D_i \leq 10^9)$�������������������������ô�����Ի��� $P_i( 1\leq P_i\leq 10^9 )$. �ڸ����Ĺ�������ͽ�ֹʱ���£�Լ���ܹ���õ��������Ϊ����.

```input1
3 
2 10 
1 5 
1 7 

```

```output1
17 

```

## ��ʾ
Complete job 3 (1,7) at time 1 and complete job 1 (2,10) at time 2 to maximize the earnings (7 + 10 -> 17).


