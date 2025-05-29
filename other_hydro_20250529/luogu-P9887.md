## ��Ŀ����
DreamGrid has just found two binary sequences $s_1, s_2, \dots, s_n$ and $t_1, t_2, \dots, t_n$ ($s_i, t_i \in \{0, 1\}$ for all $1 \le i \le n$) from his virtual machine! He would like to perform the operation described below exactly twice, so that $s_i = t_i$ holds for all $1 \le i \le n$ after the two operations.

The operation is: Select two integers $l$ and $r$ ($1 \le l \le r \le n$), change $s_i$ to $(1 - s_i)$ for all $l \le i \le r$.

DreamGrid would like to know the number of ways to do so.

We use the following rules to determine whether two ways are different:

- Let $A = (a_1, a_2, a_3, a_4)$, where $1 \le a_1 \le a_2 \le n, 1 \le a_3 \le a_4 \le n$, be a valid operation pair denoting that DreamGrid selects integers $a_1$ and $a_2$ for the first operation and integers $a_3$ and $a_4$ for the second operation;
- Let $B = (b_1, b_2, b_3, b_4)$, where $1 \le b_1 \le b_2 \le n, 1 \le b_3 \le b_4 \le n$, be another valid operation pair denoting that DreamGrid selects integers $b_1$ and $b_2$ for the first operation and integers $b_3$ and $b_4$ for the second operation.
- $A$ and $B$ are considered different, if there exists an integer $k$ ($1 \le k \le 4$) such that $a_k \ne b_k$.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$, indicating the number of test cases. For each test case:

The first line contains an integer $n$ ($1 \le n \le 10^6$), indicating the length of two binary sequences.

The second line contains a string $s_1s_2\dots s_n$ ($s_i \in \{\text{`0'}, \text{`1'}\}$) of length $n$, indicating the first binary sequence.

The third line contains a string $t_1t_2\dots t_n$ ($t_i \in \{\text{`0'}, \text{`1'}\}$) of length $n$, indicating the second binary sequence.

It's guaranteed that the sum of $n$ in all test cases will not exceed $10^7$.

## �����ʽ
For each test case, output an integer denoting the answer.

## ��Ŀ����
������������Ϊ $n$ �� **01** �ַ��� $s,\,t$������Ҫ����ж��ٸ� $1 \le l_1 \le r_1 \le n,\, 1 \le l_2 \le r_2 \le n$��ʹ�÷ֱ�**ȡ��** $s$ �������� $[l_1,\,r_1]$ ������ $[l_2,\,r_2]$ �ڵ��ַ�����$s$ �� $t$ ��ȡ�ȡ���Ķ����Ƕ��� 01 �ַ��� $a$���� $a_i = 0$ ���� $a_i \leftarrow 1$�������� $a_i \leftarrow 0$��

$1\leq n\leq 10 ^ 6$��$\sum n\leq 10 ^ 7$��

```input1
3
1
1
0
2
00
11
5
01010
00111
```

```output1
0
2
6
```

## ��ʾ
For the second sample test case, there are two valid operation pairs: $(1, 1, 2, 2)$ and $(2, 2, 1, 1)$.

For the third sample test case, there are six valid operation pairs: $(2, 3, 5, 5)$, $(5, 5, 2, 3)$, $(2, 5, 4, 4)$, $(4, 4, 2, 5)$, $(2, 4, 4, 5)$ and $(4, 5, 2, 4)$.

