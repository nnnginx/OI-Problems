## ��Ŀ����
**Note: The time limit for this problem is 4s, twice the default.**

Bessie is on vacation! Due to some recent technological advances, Bessie will travel via technologically sophisticated flights, which can even time travel. Furthermore, there are no issues if two "parallel" versions of Bessie ever meet.

In the country there are $N$ airports numbered $1,2,\cdots ,N$ and $M$ time-traveling flights $(1 \le N,M \le 200000)$. Flight $j$ leaves airport $c_j$ at time $r_j$, and arrives in airport $d_j$ at time $s_j (0 \le rj,sj \le 10^9$, $s_j<r_j$ is possible$)$. In addition, she must leave $a_i$ time for a layover at airport $i (1 \le a_i \le 10^9)$. (That is to say, if Bessie takes a flight arriving in airport $i$ at time $s$, she can then transfer to a flight leaving the airport at time $r$ if $r \ge s+a_i$. The layovers do not affect when Bessie arrives at an airport.)

Bessie starts at city $1$ at time $0$. For each airport from $1$ to $N$, what is the earliest time when Bessie can get to at it? 

## �����ʽ
The first line of input contains $N$ and $M$.

The next $M$ lines describe flights. The $j$-th of these lines contains $c_j, r_j, d_j, s_j$ in that order. $(1 \le c_j,d_j \le N, 0 \le r_j,s_j \le 10^9)$

The next line describes airports. It contains $N$
space separated integers, $a_1, \cdots ,a_N$. 

## �����ʽ
There are $N$ lines of output. Line $i$ contains the earliest time when Bessie can get to airport $i$, or $-1$ if it is not possible for Bessie to get to that airport. 

## ��Ŀ����
### ��Ŀ����

ע�⣺�����ʱ������Ϊ 4 �룬��Ĭ�����Ƶ�������

Bessie ���ڶȼ٣���������ļ���������Bessie ����ͨ���Ƚ��ĺ������У���Щ�����������Խ���ʱ�����С����⣬��ʹ���ڶ����ƽ�С��� Bessie ͬʱ����Ҳ�������κ����⡣

��������ң��� $N$ �����������Ϊ $1,2,\cdots,N$���Լ� $M$ ��ʱ�����к��ࣨ$1 \leq N,M \leq 200000$������ $j$ ������ӻ��� $c_j$ ��ʱ�� $r_j$ ��ɣ�����ʱ�� $s_j$ �ִ���� $d_j$��$0 \leq r_j,s_j \leq 10^9$��$s_j < r_j$ �ǿ��ܵģ������⣬Bessie �ڻ��� $i$ ��Ҫͣ�� $a_i$ ʱ�䣨$1 \leq a_i \leq 10^9$����Ҳ����˵����� Bessie ����һ�˺�����ʱ�� $s$ �ִ���� $i$��������ת��һ�˴Ӹû��������ĺ��ֻ࣬Ҫ�ú�������ʱ�� $r \geq s + a_i$����Ҫע����ǣ�ͣ��ʱ�䲻��Ӱ�� Bessie �ִ�ĳ������ʵ��ʱ�䡣

Bessie �ӳ��� $1$ ��������ʼʱ��Ϊ $0$�����ڴ� $1$ �� $N$ ��ÿ����������� Bessie ������Ե���û�����ʱ�䡣

### �����ʽ

��һ����������������� $N$ �� $M$��

�������� $M$ ������������Ϣ�����е� $j$ �а��� $c_j, r_j, d_j, s_j$�����α�ʾ�������ɻ��������ʱ�䡢��������ͽ���ʱ�䡣$(1 \leq c_j,d_j \leq N, 0 \leq r_j,s_j \leq 10^9)$

�������� $1$ ������ÿ��������ͣ��ʱ�䡣���а��� $N$ ���ÿո�ָ����������ֱ�Ϊ $a_1,\cdots,a_N$��

### �����ʽ

����� $N$ �С��� $i$ ����� Bessie ���絽����� $i$ ��ʱ�䣻����޷�����û�������� $-1$��

### ���� 1 �Ľ���

Bessie ���԰��ո�����˳������� $3$ �ຽ�࣬��ʹ��������ʱ�� $0$ ������� $1$ �ͻ��� $2$���Լ���ʱ�� $20$ ������� $3$��


ע�⣬����·�߻����ξ������� $2$����һ������ʱ�� $10-11$���ڶ�������ʱ�� $0-1$��

### ���� 2 �Ľ���

����������У�Bessie ���Գ����� $1$ �ຽ�࣬��ʱ�� $10$ �ִ���� $2$�����ǣ����޷���ʱ���ϵ� $2$ �ຽ�࣬��Ϊ�ú�������ʱ��Ϊ $10$��������Ҫ���� $1$ ��ʱ�䵥λ�����ͣ����

### ���ֱ�׼

 - ���Ե� $3-5$������ÿ�� $j$��$r_j < s_j$��Ҳ����˵���к���ĵ���ʱ���������ʱ�䡣
 - ���Ե� $6-10$��$N,M \leq 5000$
 - ���Ե� $11-20$���޶������ơ�

```input1
3 3
1 0 2 10
2 11 2 0
2 1 3 20
10 1 10
```

```output1
0
0
20
```

```input2
3 3
1 0 2 10
2 10 2 0
2 1 3 20
10 1 10
```

```output2
0
10
-1
```

## ��ʾ
### Explanation for Sample 1

Bessie can take the $3$ flights in the listed order, which allows her to arrive at airports $1$ and $2$ at time $0$, and airport $3$ at time $20$.

Note that this route passes through airport $2$ twice, first from time $10-11$ and then from time $0-1$.

### Explanation for Sample 2

In this case, Bessie can take flight $1$, arriving at airport $2$ at time $10$. However, she does not arrive in time to also take flight $2$, since the departure time is $10$ and she cannot make a $1$ time-unit layover. 

### SCORING

 - Inputs $3-5$: $r_j<s_j$ for all $j$, i.e. all flights arrive after they depart.
 - Inputs $6-10$: $N,M \le 5000$
 - Inputs $11-20$: No additional constraints.

