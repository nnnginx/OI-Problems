## ��Ŀ����
The Byteotian Software Corporation (BSC) has $n$ employees.

In BSC's strict hierarchy, each employee has a direct supervisor, except the CEO, to whom all other BSC employees answer, directly or not.

Each employee has a unique monthly salary, and all their salaries range from 1 to $n$ bythalers.

Each supervisor earns more than each of their subordinates.

According to Byteotian law, the salaries of employees on certain posts may be publicly disclosed.

Furthermore, if the salary of an employee is disclosed, then the salary of their supervisor is also disclosed.

The Byteotian Internal Revenue Anti-Corruption Service (BIRAS) has decided to investigate BSC.

Before BIRAS enters BSC with a warrant, they intend to learn the salaries of all BSC employees    that are not disclosed but can be determined from those that are disclosed.

## �����ʽ
In the first line of the standard input a single integer $n$ ($1\le n\le 1\ 000\ 000$) is given that denotes the number of BSC employees.

The employees have id's that range from 1 to $n$.

The $n$ lines that follow provide information on these employees.

The line no. $i+1$ describes the employee no. $i$ by two integers $p_i$ and $z_i$ ($1\le p_i\le n$, $0\le z_i\le n$), separated by a single space.

The number $p_i$ is the id of the direct supervisor of the employee $i$.If $p_i=i$, then $i$ is the CEO of BSC. If $z_i>0$,then that is the salary of the employee $i$.If, on the other hand,$z_i=0$, then the salary of employee $i$ is not disclosed.Those $z_i$'s that are positive are also pairwise different.

The input data will always be such that there is at least one assignment of salaries to employees consistent with them, i.e., with the hierarchy and the partial assignment that they provide.

In tests worth 54% of the total points the condition $n\le 10\ 000$  holds in addition.


## �����ʽ
Your program should print $n$ lines to the standard output, each line holding a single integer.

If the employee $i$'s salary is disclosed or can be inferred from disclosed salaries, then the $i$-th line should hold employee $i$'s salary.

Otherwise the $i$-th line should contain $0$.


## ��Ŀ����
### ��Ŀ����

**���� POI 2012 Stage 3. Day 1��[Salaries](https://szkopul.edu.pl/problemset/problem/_qn633f6DVAHRkv0OX3LQaph/site/?key=statement)��**

��һ�� $n$ ������и�����ÿ�����Ȩֵ�ֱ�Ϊ $1 \ldots n$���Ҵ�������ӵ�Ȩֵ������һ���ֵ��Ȩֵ�ǹ����ģ���ÿ��Ȩֵ��֪�ĵ�ĸ���ȨֵҲһ����֪�����ܹ�������֪��Ϣ���������Ȩֵδ֪�ĵ��Ȩֵ��

### �����ʽ

��һ��һ������ $n$����ʾ��ĸ�����

������ $n$ ��ÿ���������� $p_i, z_i (1 \le p_i \le n,0 \le z_i \le n)$������ $p_i$ ��ʾ��� $i$ �ĸ��ף�$z_i$ ��ʾ��� $i$ ��Ȩֵ����� $z_i = 0$����õ�Ȩֵδ֪������õ�ȨֵΪ $z_i$��

### �����ʽ

��� $n$ �У�ÿ��һ����������ʾ $i$ ���Ȩֵ������õ�Ȩֵ��֪������������������õ�Ȩֵ��������� $0$��

### ��������

![](https://cdn.luogu.com.cn/upload/image_hosting/bjf4memv.png)

### ���ݷ�Χ

���� $54\%$ �������� $n \le 10^4$.

�������������� $1 \le n \le 10^6$��

���������� [LibreOJ](https://loj.ac/p/2700)��

```input1
10
2 2
2 10
1 0
2 9
2 5
4 0
6 0
6 0
5 0
5 0
```

```output1
2
10
1
9
5
8
0
0
0
0
```

