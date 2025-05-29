## ��Ŀ����
**Warning: Unusual memory limit!**

You are given a sequence $a_0,\ldots,a_{2n}$. Initially, all numbers are zero. 

There are $n$ operations. The $i$-th operation is represented by two integers $l_i, r_i$ ($1\le l_i < r_i\le 2n, 1\le i\le n$), which assigns $i$ to $a_{l_i},\ldots,a_{r_i-1}$.  It is guaranteed that all the $2n$ integers, $l_1,l_2,\ldots, l_n, r_1, r_2, \ldots, r_n$, are distinct.

You need to perform each operation exactly once, in arbitrary order.

You want to maximize the number of $i$ $(0\leq i< 2n)$ such that $a_i\neq a_{i+1}$ after all $n$ operations. Output the maximum number.

## �����ʽ
The first line contains an integer $n$ ($1\le n\le 5\times 10^3$).

The $i$-th line of the next $n$ lines contains a pair of integers $l_i, r_i$ ($1\le l_i < r_i\le 2n$). It is guaranteed that all the $2n$ integers, $l_1,l_2,\ldots, l_n, r_1, r_2, \ldots, r_n$, are distinct.

## �����ʽ
Output one integer representing the answer in one line.

## ��Ŀ����
- ����һ������ $a_0,a_1,a_2\dots a_{2n}$����ʼȫΪ $0$��
- ���� $n$ �����丳ֵ�������� $i$ ������ $(l_i,r_i)(1\le l_i,r_i\le 2n)$ ��ʾ������ $[l_i,r_i)$ ȫ����ֵΪ $i$��**��֤���� $l_i,r_i$ ������ͬ**��
- �����ָ��һ��ִ�в�����˳����� $\sum_{i=0}^{2n-1}[a_i\ne a_{i+1}]$�����������ֵ��
- $1\le n\le 5\times 10^3$��**ע��ռ�����**��

```input1
5
2 3
6 7
1 9
5 10
4 8

```

```output1
9

```

