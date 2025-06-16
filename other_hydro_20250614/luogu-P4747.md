## ��Ŀ����
Given a permutation $\pi$ of integers $1$ through $n$, an interval in $\pi$ is a consecutive subsequence consisting of consecutive numbers. More precisely, for indices $a$ and $b$ where $1 \le a \le b \le n$, the subsequence $\pi^b_a = (\pi_a, \pi_{a+1}, . . . ,\pi_b)$ is an interval if sorting it would yield a sequence of consecutive integers.

For example, in permutation $\pi = (3, 1, 7, 5, 6, 4, 2)$, the subsequence $\pi^6_3$ is an interval (it contains the numbers $4$ through $7$) while $\pi^3_1$ is not.

For a subsequence $\pi^y_x$ its intrinsic interval is any interval $\pi^b_a$ that contains the given subsequence $(a \le x \le y \le b)$ and that is, additionally, as short as possible. Of course, the length of an interval is defined as the number of elements it contains.

Given a permutation $\pi$ and $m$ of its subsequences, find some intrinsic interval for each subsequence.

## �����ʽ
The first line contains an integer $n(1 \le n \le 100 000)$ �� the size of the permutation $\pi$. The following line contains $n$ different integers $\pi_1, \pi_2, . . . , \pi_n (1 \le \pi_j \le n)$ �� the permutation itself.

The following line contains an integer $m(1 \le m \le 100 000)$ �� the number of subsequences. The $j-th$ of the following $m$ lines contains integers $x_j$ and $y_j(1 \le x_j \le y_j \le n)$ �� the endpoints of the $j-th$ subsequence.


## �����ʽ
Output $m$ lines. The $j-th$ line should contain two integers $a_j$ and $b_j$ where $1 \le a_j \le b_j \le n$ �� the endpoints of some intrinsic interval of the $j-th$ subsequence $\pi^{y_j}_{x_j}$.

## ��Ŀ����
### ��Ŀ����

���������� $1,2,3 \cdots n$ ��һ������ $\pi$��������һ���Ӵ� $\pi[a..b]$ ���������������������� $\pi[a..b]$ ��һ�������䡱����������� $pi={3,1,7,5,6,4,2}$���Ӵ� $\pi[3..6]$ ��һ�������䡱����Ϊ������ $4,5,6,7$����$\pi[1..3]$ ���ǡ�

һ���Ӵ��ġ��������䡱�ǰ������Ӵ���������䡣����������ָ���� $\pi[x..y]$ �ı��������� $\pi[a..b]$���� $a \le x \le y \le b$��

����һ������ $\pi$ ���� $m$ ���Ӵ�����ÿ���Ӵ��ġ��������䡱��

### �����ʽ

��һ��һ������ $n(1 \le n \le 100000)$��

�ڶ��� $n$ ���������������� $\pi$��

������һ������ $m(1 \le m \le 100000)$��

�˺� $m$ �У�ÿ���������� $x,y(1 \le x \le y \le n)$�������Ӵ� $\pi[x..y]$��

### �����ʽ

��� $m$ �У�ÿ���������� $a,b(1 \le a \le b \le n)$�������Ӵ���Ӧ�ı������� $\pi[a..b]$��



```input1
7
3 1 7 5 6 4 2
3
3 6
7 7
1 3

```

```output1
3 6
7 7 
1 7
```

```input2
10
2 1 4 3 5 6 7 10 8 9
5
2 3
3 7
4 7
4 8
7 8

```

```output2
1 4
3 7
3 7
3 10
7 10

```

