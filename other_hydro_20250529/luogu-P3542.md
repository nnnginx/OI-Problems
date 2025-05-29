## 题目描述
The Byteotian Software Corporation (BSC) has $n$ employees.

In BSC's strict hierarchy, each employee has a direct supervisor, except the CEO, to whom all other BSC employees answer, directly or not.

Each employee has a unique monthly salary, and all their salaries range from 1 to $n$ bythalers.

Each supervisor earns more than each of their subordinates.

According to Byteotian law, the salaries of employees on certain posts may be publicly disclosed.

Furthermore, if the salary of an employee is disclosed, then the salary of their supervisor is also disclosed.

The Byteotian Internal Revenue Anti-Corruption Service (BIRAS) has decided to investigate BSC.

Before BIRAS enters BSC with a warrant, they intend to learn the salaries of all BSC employees    that are not disclosed but can be determined from those that are disclosed.

## 输入格式
In the first line of the standard input a single integer $n$ ($1\le n\le 1\ 000\ 000$) is given that denotes the number of BSC employees.

The employees have id's that range from 1 to $n$.

The $n$ lines that follow provide information on these employees.

The line no. $i+1$ describes the employee no. $i$ by two integers $p_i$ and $z_i$ ($1\le p_i\le n$, $0\le z_i\le n$), separated by a single space.

The number $p_i$ is the id of the direct supervisor of the employee $i$.If $p_i=i$, then $i$ is the CEO of BSC. If $z_i>0$,then that is the salary of the employee $i$.If, on the other hand,$z_i=0$, then the salary of employee $i$ is not disclosed.Those $z_i$'s that are positive are also pairwise different.

The input data will always be such that there is at least one assignment of salaries to employees consistent with them, i.e., with the hierarchy and the partial assignment that they provide.

In tests worth 54% of the total points the condition $n\le 10\ 000$  holds in addition.


## 输出格式
Your program should print $n$ lines to the standard output, each line holding a single integer.

If the employee $i$'s salary is disclosed or can be inferred from disclosed salaries, then the $i$-th line should hold employee $i$'s salary.

Otherwise the $i$-th line should contain $0$.


## 题目大意
### 题目描述

**译自 POI 2012 Stage 3. Day 1「[Salaries](https://szkopul.edu.pl/problemset/problem/_qn633f6DVAHRkv0OX3LQaph/site/?key=statement)」**

有一个 $n$ 个点的有根树，每个点的权值分别为 $1 \ldots n$，且大于其儿子的权值。其中一部分点的权值是公开的，且每个权值已知的点的父亲权值也一定已知。求能够根据已知信息推算出来的权值未知的点的权值。

### 输入格式

第一行一个整数 $n$，表示点的个数。

接下来 $n$ 行每行两个整数 $p_i, z_i (1 \le p_i \le n,0 \le z_i \le n)$，其中 $p_i$ 表示结点 $i$ 的父亲，$z_i$ 表示结点 $i$ 的权值。如果 $z_i = 0$，则该点权值未知，否则该点权值为 $z_i$。

### 输出格式

输出 $n$ 行，每行一个整数，表示 $i$ 点的权值。如果该点权值已知或可以推算出来，输出该点权值，否则输出 $0$。

### 样例解释

![](https://cdn.luogu.com.cn/upload/image_hosting/bjf4memv.png)

### 数据范围

对于 $54\%$ 的数据有 $n \le 10^4$.

对于所有数据有 $1 \le n \le 10^6$。

翻译来自于 [LibreOJ](https://loj.ac/p/2700)。

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

