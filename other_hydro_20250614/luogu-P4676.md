## ��Ŀ����
A grid of size $(2n+1)\times(2n+1)$ has been constructed as follows. Number $1$ has been placed in the center square, number $2$ has been placed to the right of it, and the following numbers have been placed along the spiral counterclockwise.

Your task is to calculate answers for $q$ queries where the sum of numbers in an rectangular region in the grid is requested (modulo $10^9+7$). For example, in the following grid $n=2$ and the sum of numbers in the gray region is $74$ :

![](https://cdn.luogu.com.cn/upload/pic/20871.png)

## �����ʽ
The first input line contains two integers $n$ and $q$ : the size of the grid and the number of queries.

After this, there are $q$ lines, each containing four integers $x_1, y_1, x_2$  and $y_2$ ($-n\leq x_1\leq x_2\leq n, -n\leq y_1\leq y_2\leq n$). This means that you should calculate the sum of numbers in a rectangular region with corners $(x_1,y_1)$ and $(x_2,y_2)$.

## �����ʽ
You should output the answer for each query (modulo $10^9+7$).


## ��Ŀ����
[BalticOI 2016 Day1]����

## ��Ŀ����

һ������Ĵ�СΪ $(2n+1)\times (2n+1)$��������ͨ�������������������� $1$ �����ģ����� $2$ �����ң������������ΰ�����ʱ�������ڷš�

��������Ƕ��� $q$ ��ѯ�ʣ������һ�������Ӿ����������ֵĺͶ� $(10^9+7)$ ȡ��Ľ������������ $n=2$ �ľ��󣬻�ɫ���������֮��Ϊ $74$��

![](https://i.loli.net/2018/08/11/5b6e3ead24175.png)

## �����ʽ

��һ�У��������� $n$ �� $q$���ֱ��ʾ����Ĵ�С��ѯ�ʵĸ�����

������ $q$ �У�ÿ���ĸ����� $x_1,y_1,x_2$ �� $y_2$ $(-n \leq x_1 \leq x_2 \leq n,$ $-n \leq y_1 \leq y_2 \leq n)$�����ʾ����Ҫ����һ���Խ�Ϊ $(x_1,y_1)$ �� $(x_2,y_2)$ ���Ӿ��������֮�͡�

## �����ʽ

����ÿ��ѯ�ʣ����һ�б�ʾ�𰸣��� $10^9+7$ ȡ�ࣩ��

�� @I_love_him52 �ṩ����

```input1
2 3
0 -2 1 1
-1 0 1 0
1 2 1 2

```

```output1
74
9
14

```

## ��ʾ
## Subtasks

In all subtasks $1\leq q\leq100$.

### Subtask 1 (12 points)

- $1\leq n\leq1000$

### Subtask 2 (15 points)

- $1\leq n\leq10^9$

- $x_1=x_2$ and $y_1=y_2$

### Subtask 3 (17 points)

- $1\leq n\leq10^5$

### Subtask 4 (31 points)

- $1\leq n\leq10^9$

- $x_1=y_1=1$

### Subtask 5 (25 points)

- $1\leq n\leq10^9$


