## ��Ŀ����

A suffix array for string $s$ of length $n$ is a permutation $sa$ of integers from $1$ to $n$ such that $s[sa_1.. n], s[sa_2..n], \dots, s[sa_n..n]$ is the list of non-empty suffixes of $s$ sorted in lexicographical order. The rank table for suffixex of $s$ is a permutation $rank$ of integers from $1$ to $n$ such that $rank_{sa_i} = i$.

Kotori has a string $s=s_1s_2\dots s_n$. She would like to ask $m$ queries. And in the $i$-th query, a substring $x=s[l_i..r_i]$ of $s$ is given, Kotori would like to know the rank of suffix $s[k_i..r_i]$ of $x$.

Note $s[l..r]$ means the substring of $s$ which starts from the $l$-th position and ends at the $r$-th position, both inclusive.


## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ indicating the number of test cases. For each test case:

The first line contains two integers $n$ and $m$ ($1 \le n, m \le 5 \times 10^4$) -- the length of the string and the number of queries.

The second line contains a string $s$ of length $n$ consisting only of lowercase English letters.

Each of the next $m$ lines contains three integers $l_i$, $r_i$ and $k_i$ ($1 \le l_i \le r_i \le n, l_i \le k_i \le r_i$) denoting a query.

It is guaranteed that neither the sum of $n$ or the sum of $m$ of all test cases will exceed $5 \times 10^4$.

## �����ʽ
For each query output one line containing one integer denoting the answer.

## ��Ŀ����
��һ������Ϊ $n$ ���ַ��� $s=[s_1,s_2,..,s_n]$���� $m$ ��ѯ�ʣ�ÿ��ѯ�ʸ��� $l,r,k$���ֽ� $s$ ���Ӵ� $[s_l,..,s_r]$ �� $r-l+1$ ����׺�ַ������ֵ����С���������� $[s_k,..,s_r]$ �����е�������

�� $T$ �����ݡ�

���ݱ�֤ $1 \leq n,m,\sum n,\sum m \leq 5 \times 10^4$������ÿ��ѯ�ʣ���֤ $1 \leq l \leq k \leq r \leq n$��

```input1
2
10 4
baaabbabba
2 8 3
1 1 1
2 3 2
2 5 4
20 3
cccbccbadaacbbbcccab
14 17 16
3 20 17
17 20 18

```

```output1
2
1
2
3
4
15
3

```

