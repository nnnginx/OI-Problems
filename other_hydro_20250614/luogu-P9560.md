## ��Ŀ����
Given two positive integers $n$ and $k$, you can perform the following two types of operations any number of times (including zero times):

- Choose an integer $x$ which satisfies $0 \leq x < k$, and change $n$ into $k\cdot n+x$. It will cost you $a$ coins to perform this operation once. The integer $x$ you choose each time can be different.
- Change $n$ into $\lfloor \frac{n}{k} \rfloor$. It will cost you $b$ coins to perform this operation once. Note that $\lfloor \frac{n}{k} \rfloor$ is the largest integer which is less than or equal to $\frac{n}{k}$.

Given a positive integer $m$, calculate the minimum number of coins needed to change $n$ into a multiple of $m$. Please note that $0$ is a multiple of any positive integer.


## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ ($1\leq T\leq 10^5$) indicating the number of test cases. For each test case:

The first line contains five integers $n$, $k$, $m$, $a$, $b$ ($1\leq n\leq 10^{18}$, $1\leq k, m, a, b\leq 10^9$).

## �����ʽ
For each test case output one line containing one integer, indicating the minimum number of coins needed to change $n$ into a multiple of $m$. If this goal cannot be achieved, output $-1$ instead.

## ��Ŀ����
**����Ŀ������**

�������������� $n$ �� $k$�������Խ����������ֲ�������Σ�������Σ���

- ѡ��һ������ $x$ ���� $0 \leq x < k$���� $n$ ��Ϊ $k\cdot n+x$���ò���ÿ�λ��� $a$ ö��ҡ�ÿ��ѡ������� $x$ ���Բ�ͬ��
- �� $n$ ��Ϊ $\lfloor \frac{n}{k} \rfloor$���ò���ÿ�λ��� $b$ ö��ҡ����� $\lfloor \frac{n}{k} \rfloor$ ��ʾС�ڵ��� $\frac{n}{k}$ �����������

���������� $m$���� $n$ ��Ϊ $m$ �ı���������Ҫ���Ѽ�ö��ҡ���ע�⣺$0$ ���κ��������ı�����

**�������ʽ��**

�ж���������ݡ���һ������һ������ $T$��$1\leq T\leq 10^5$����ʾ������������������ÿ��������ݣ�

��һ��������������� $n$��$k$��$m$��$a$��$b$��$1\leq n\leq 10^{18}$��$1\leq k, m, a, b\leq 10^9$����

**�������ʽ��**

ÿ���������һ��һ������������ $n$ ��Ϊ $m$ �ı���������Ҫ���Ѽ�ö��ҡ�����޷���ɸ�Ŀ�꣬��� $-1$��

**���������͡�**

���ڵ�һ���������ݣ�һ��ʼ $n=101$�����Ų������£�

- ���Ƚ���һ�εڶ��ֲ������� $n$ ��Ϊ $\lfloor \frac{n}{4} \rfloor=25$������ $5$ ö��ҡ�
- ����������һ�ε�һ�ֲ�����ѡ�� $x = 3$���� $n$ ��Ϊ $4\cdot n+3=103$������ $3$ ö��ҡ�
- ����������һ�ε�һ�ֲ�����ѡ�� $x = 2$���� $n$ ��Ϊ $4\cdot n+2=414$������ $3$ ö��ҡ�
- ��ʱ $414=2 \times 207$������ $n$ �� $m$ �ı����������� $5+3+3=11$ ö��ҡ�

���ڵڶ����������ݣ��������εڶ��ֲ����� $n$ ��Ϊ $0$�������� $1 + 1 = 2$ ö��ҡ�

���ڵ������������ݣ���Ϊ $n = 114 = 6 \times 19$ �Ѿ��� $m$ �ı����������������κβ����������� $0$ ö��ҡ�

```input1
4
101 4 207 3 5
8 3 16 100 1
114 514 19 19 810
1 1 3 1 1
```

```output1
11
2
0
-1
```

## ��ʾ
For the first sample test case, initially $n=101$. The optimal steps are shown as follows:

- Firstly, perform the second type of operation once. Change $n$ into $\lfloor \frac{n}{4} \rfloor=25$. This step costs $5$ coins.
- Then, perform the first type of operation once. Choose $x = 3$ and change $n$ into $4\cdot n+3=103$. This step costs $3$ coins.
- Then, perform the first type of operation once. Choose $x = 2$ and change $n$ into $4\cdot n+2=414$. This step costs $3$ coins.
- As $414=2 \times 207$, $n$ is a multiple of $m$. The total cost is $5+3+3=11$ coins.

For the second sample test case, perform the second type of operation twice will change $n$ into $0$. The total cost is $1 + 1 = 2$ coins.

For the third sample test case, as $n = 114 = 6 \times 19$ is already a multiple of $m$, no operation is needed. The total cost is $0$ coins.

