## ��Ŀ����

Prof. Pang has $3$ different skills to practice, including soda drinking, fox hunting, and stock investing. We call them Skill $1$, Skill $2$, and Skill $3$. In each of the following $n$ days, Prof. Pang can choose one of the three skills to practice. In the $i$-th day ($1\le i\le n$), if Prof. Pang chooses Skill $j$ ($1\le j\le 3$) to practice, his level of Skill $j$ will increase by $a_{i,j}$. Initially, Prof. Pang's levels of all skills are $0$.

Prof. Pang forgets skills if he does not practice. At the end of each day, if he has not practiced Skill $j$ for $k$ days, his level of Skill $j$ will decrease by $k$. For example, if he practices Skill $1$ on day $1$ and Skill $2$ on day $2$, at the end of day $2$, he has not practiced Skill $1$ for $1$ day and has not practiced Skill $3$ for $2$ days. Then his levels of Skill $1$ and Skill $3$ will decrease by $1$ and $2$, respectively. His level of Skill $2$ does not decrease at the end of day $2$ because he practices Skill $2$ on that day. In this example, we also know that his levels of Skill $2$ and Skill $3$ both decrease by $1$ at the end of day $1$.

Prof. Pang's level of any skill will not decrease below $0$. For example, if his level of some skill is $3$ and at the end of some day, this level is decreased by $4$, it will become $0$ instead of $-1$.

Prof. Pang values all skills equally. Thus, he wants to maximize the sum of his three skill levels after the end of day $n$. 

Given $a_{i,j}$ ($1\le i\le n, 1\le j\le 3$), find the maximum sum.


## �����ʽ
The first line contains a single integer $T~(1 \le T \le 1000)$ denoting the number of test cases.

For each test case, the first line contains an integer $n~(1 \le n \le 1000)$. The $(i+1)$-th line contains three integers $a_{i,1}, a_{i,2}, a_{i,3}$ ($0\le a_{i,j}\le 10000$ for any $1\le i\le n, 1\le j\le 3$).

It is guaranteed that the sum of $n$ over all test cases is no more than $1000$.

## �����ʽ
For each test case, output the maximum possible sum of skill levels in one line. 

## ��Ŀ����
#### ��Ŀ������
�Ӳ�ʿ�� $3$ ��ܣ�����ˮ���Ժ��ͳ��ɣ���ŷֱ�Ϊ $1,2,3$����ʼʱ��ÿ��ܵ�������Ϊ $0$��

�������� $n$ �졣�ڵ� $i$ �죬�Ӳ�ʿ����ѡ��һ��ܣ������ǵ� $j$ �������ϰ��Ȼ�����������ʱ������ܵ����������� $a_{i,j}$��ͬʱ�����ĳһ��ܣ������ǵ� $k$ ��Ѿ��� $x$ ��û����ϰ����ô���������ʱ������ܵ������Ȼ���� $x$����Ȼ���κ�һ��ܵ������ȶ�������С�� $0$��

���ڣ��Ӳ�ʿ��֪�����ڵ� $n$ ��������� $3$ ��ܵ�������֮�����Ϊ���١��������ǳ�æ�����������ճ̺Ͷ�ϰ�ߵ���Ӧ�̶ȿ����б䣬�����Ӳ�ʿ���� $T$ �����⽻�����㡪��ÿ����������ݶ�һ����ֻ�Ǹ��������ݿ���������ͬ���ѡ�
#### �����ʽ
��һ�У�һ�������� $T~(1 \leq T \leq 1000)$����ʾ����������

����ÿ�����ݣ����� $(n + 1)$ �С�

* ��һ�У�һ�������� $n~(1 \leq n \leq 1000)$����ʾ������

* ������ $n$ �У�ÿ�� $3$ ���Ǹ���������ʾ��Ŀ�����е� $a_{i,j}~(1 \leq i \leq n,1 \leq j \leq 3,0 \leq a_{i,j} \leq 10000)$��
#### �����ʽ
����ÿ�����ݣ���� $1$ �� $1$ ��������ʾ�𰸡�

```input1
2
3
1 1 10
1 10 1
10 1 1
5
1 2 3
6 5 4
7 8 9
12 11 10
13 14 15

```

```output1
26
41
```

