## ��Ŀ����
Paimon just learns the persistent segment tree and decides to practice immediately. Therefore, Lumine gives her an easy problem to start:

Given a sequence $a_1, a_2, \cdots, a_n$ of length $n$, Lumine will apply $m$ modifications to the sequence. In the $i$-th modification, indicated by three integers $l_i$, $r_i$ ($1 \le l_i \le r_i \le n$) and $x_i$, Lumine will change $a_k$ to $(a_k + x_i)$ for all $l_i \le k \le r_i$.

Let $a_{i, t}$ be the value of $a_i$ just after the $t$-th operation. This way we can keep track of all historial versions of $a_i$. Note that $a_{i,t}$ might be the same as $a_{i,t-1}$ if it hasn't been modified in the $t$-th modification. For completeness we also define $a_{i, 0}$ as the initial value of $a_i$.

After all modifications have been applied, Lumine will give Paimon $q$ queries about the sum of squares among the historical values. The $k$-th query is indicated by four integers $l_k$, $r_k$, $x_k$ and $y_k$ and requires Paimon to calculate

$$\sum\limits_{i=l_k}^{r_k}\sum\limits_{j=x_k}^{y_k} a_{i, j}^2$$

Please help Paimon compute the result for all queries. As the answer might be very large, please output the answer modulo $10^9 + 7$.

## �����ʽ
There is only one test case in each test file.

The first line of the input contains three integers $n$, $m$ and $q$ ($1 \le n, m, q \le 5 \times 10^4$) indicating the length of the sequence, the number of modifications and the number of queries.

The second line contains $n$ integers $a_1, a_2, \cdots, a_n$ ($|a_i| < 10^9 + 7$) indicating the initial sequence.

For the following $m$ lines, the $i$-th line contains three integers $l_i$, $r_i$ and $x_i$ ($1 \le l_i \le r_i \le n$, $|x_i| < 10^9 + 7$) indicating the $i$-th modification.

For the following $q$ lines, the $i$-th line contains four integers $l_i$, $r_i$, $x_i$ and $y_i$ ($1 \le l_i \le r_i \le n$, $0 \le x_i \le y_i \le m$) indicating the $i$-th query.

## �����ʽ
For each query output one line containing one integer indicating the answer modulo $10^9 + 7$.

## ��Ŀ����
## ��Ŀ����

���ɸո�ѧϰ�˿ɳ־û��߶���������������ϰһ�¡���ˣ�ӫ����������һ���򵥵����⣺

��������$a_1, a_2, \cdots, a_n$��������$m$�β�������������3������$l_i$, $r_i$ ($1 \le l_i \le r_i \le n$) �� $x_i$������Ը����е�$l_i$����$r_i$��Ԫ�ؼ���$x_i$��

��$a_{i, t}$Ϊ$t$�β�����$a_i$��ֵ��ע����$a_i$δ���޸ģ���$a_{i,t}$��ֵ��$a_{i,t-1}$��ͬ������$a_{i, 0}$��$a_i$�ĳ�ʼֵ��


������в�����ӫ����$q$��ѯ�ʣ�ѯ�ʰ���4������$l_k$, $r_k$, $x_k$ and $y_k$��������Ҫ�ش�

$$\sum\limits_{i=l_k}^{r_k}\sum\limits_{j=x_k}^{y_k} a_{i, j}^2$$

�뽫�𰸶�$10^9 + 7$ȡģ�������

## �����ʽ
ÿ�����Ե㺬һ��������ݡ�

��һ��3������$n$,$m$,$q$ ($1 \le n, m, q \le 5 \times 10^4$) �ֱ��ʾ���еĳ��ȣ������Ĵ�����ѯ�ʵĴ�����

��2��$n$������ $a_1, a_2, \cdots, a_n$ ($|a_i| < 10^9 + 7$) ����ʾԭʼ���С�

������$m$��ÿ��3������ $l_i$, $r_i$ $x_i$ ($1 \le l_i \le r_i \le n$, $|x_i| < 10^9 + 7$)����ʾ����Ӳ�����

������$q$��ÿ�а����ĸ����� $l_i$, $r_i$, $x_i$  $y_i$ ($1 \le l_i \le r_i \le n$, $0 \le x_i \le y_i \le m$)����ʾѯ�ʡ�

## �����ʽ

��ÿ��ѯ�ʵ���һ�������ģ$10^9 + 7$�Ľ����

```input1
3 1 1
8 1 6
2 3 2
2 2 0 0

```

```output1
1

```

```input2
4 3 3
2 3 2 2
1 1 6
1 3 3
1 3 6
2 2 2 3
1 4 1 3
4 4 2 3

```

```output2
180
825
8

```

