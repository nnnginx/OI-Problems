## ��Ŀ����
Prof. Pang builds his famous coding team recently. To pursue a gold medal in ICPC, hundreds of pupils join his team. Unfortunately, one of Prof. Pang's students believes that for any integers $a$ and $b$, $a\times b\ge a+b$. To disprove this proposition, Prof. Pang writes $n$ numbers $a_1,a_2,\ldots, a_n$ on a paper and wants you to count how many pairs of numbers $(a_i, a_j)$ ($1\le i < j\le n$) satisfies $a_i\times a_j<a_i+a_j$.

## �����ʽ
The first line contains a single integer $T$ ($1\le T\le 10^6$) denoting the number of test cases.

For each test case, the first line contains a single integer $n$ ($1\le n\le 10^6$). The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9\le a_i\le 10^9$).

It is guaranteed that the sum of $n$ over all test cases will not exceed $10^6$.

## �����ʽ
For each test case, print one line containing the answer.

## ��Ŀ����
### ��Ŀ����

�� $T$ �����ݣ�ÿ�����һ���� $n$ �� $n$ ���� $a_1,a_2,...,a_n$�����ж��ٸ���Ԫ�� $(a_i,a_j)$ ���� $a_ia_j<a_i+a_j$��

### �����ʽ

��һ��Ϊһ���� $T$��

������ $T$ �����ݣ�ÿ�����ݵ�һ��Ϊһ���� $n$���ڶ���Ϊ $n$ ���� $a_1,a_2,...,a_n$��

### �����ʽ

$T$ �У�Ϊ���� $a_ia_j<a_i+a_j$ �Ķ�Ԫ�� $(a_i,a_j)$ ��������

Translated from [FurippuWRY](https://www.luogu.com.cn/user/993779)��

```input1
2
8
3 -1 4 1 -5 9 2 -6
1
0

```

```output1
19
0

```

