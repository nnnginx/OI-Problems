## ��Ŀ����
There are $n$ cells arranged in a row. The $i$-th cell has a color $c_i$ and contains a ball with value $v_i$.

You're going to travel several times in the cells. For each travel, you'll be given an integer $x$ and a set of colors $\mathbb{A} = \{a_1, a_2, \cdots, a_k\}$ where $c_x \in \mathbb{A}$. The travel starts from cell $x$. During the travel, if you're located in cell $i$ you can next move to cell $(i - 1)$ or $(i + 1)$. Note that you can't move out of these $n$ cells. Also at any time, the color of cell you're located in must belong to set $\mathbb{A}$.

When you're in cell $i$, you can choose to remove the ball in the cell and gain its value $v_i$. As there is only one ball in each cell, you can only remove the ball from each cell once.

Your task is to process $q$ operations in order. Each operation is one of the following three types:

- $1\; p \; x$: Change $c_p$ to $x$.
- $2\; p \; x$: Change $v_p$ to $x$.
- $3\; x\; k\; a_1\; a_2 \; \ldots\; a_k$: Given the starting cell $x$ and the color set $\mathbb{A} = \{a_1, a_2, \cdots, a_k\}$ of a travel, imagine that you're going on this travel, calculate the maximum total value you can gain. Note that this travel is only an imagination, thus the balls won't be truely removed. That is, all queries are independent.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ indicating the number of test cases. For each test case:

The first line contains two integers $n$ and $q$ ($1 \leq n \leq 10^5$, $1 \leq q \leq 10^5$) indicating the number of cells and the number of operations.

The second line contains $n$ integers $c_1, c_2, \ldots, c_n$ ($1 \leq c_i \leq n$) where $c_i$ is the initial color of the $i$-th cell.

The third line contains $n$ integers $v_1, v_2, \ldots, v_n$ ($1 \leq v_i \leq 10^9$) where $v_i$ is the initial value of ball in the $i$-th cell.

For the following $q$ lines, the $i$-th line describes the $i$-th operation. The input format is listed as follows:

- $1\; p\; x$: $1 \leq p \leq n$ and $1 \leq x \leq n$.
- $2\; p\; x$: $1 \leq p \leq n$ and $1 \leq x \leq 10^9$.
- $3\; x\; k\; a_1\; a_2\; \ldots \; a_k$: $1 \leq x \leq n$, $1 \leq a_1 < a_2 < \ldots < a_k \leq n$ and $c_x \in \{a_1, a_2, \cdots, a_k\}$.

It's guaranteed that neither the sum of $n$ nor the sum of $q$ of all test cases will exceed $3 \times 10^5$. Also the sum of $k$ of all test cases will not exceed $10^6$.

## �����ʽ
For each operation of type $3$ output one line containing one integer, indicating the maximum total value you can gain.

## ��Ŀ����
**����Ŀ������**

�� $n$ �������ų�һ�У��� $i$ �����ӵ���ɫΪ $c_i$�����������һ��ȨֵΪ $v_i$ ����

����Ҫ�ڸ����н������ɴ����С�ÿ������ʱ������õ����е���� $x$ ��һ����ɫ���� $\mathbb{A} = \{a_1, a_2, \cdots, a_k\}$���ұ�֤ $c_x \in \mathbb{A}$�����н��ӵ� $x$ �������Ͽ�ʼ���������ڼ䣬������ڸ��� $i$ ������ô����������� $(i - 1)$ �� $(i + 1)$ ���ƶ����������ƶ����� $n$ ������֮�⡣��������ʱ�̣��������ĸ��ӵ���ɫ�����ڼ��� $\mathbb{A}$ �С�

����λ�ڸ��� $i$ ʱ��������ѡ�񽫸����ϵ���ȡ�ߣ������ $v_i$ ��Ȩֵ������ÿ��������ֻ��һ�������һ�������ϵ���ֻ�ܱ�ȡ��һ�Ρ�

�������������δ��� $q$ �β�����ÿ�β��������������ֲ���֮һ��

- $1\; p \; x$���� $c_p$ �޸�Ϊ $x$��
- $2\; p \; x$���� $v_p$ �޸�Ϊ $x$��
- $3\; x\; k\; a_1\; a_2 \; \ldots\; a_k$���������е���� $x$ ��һ����ɫ���� $\mathbb{A} = \{a_1, a_2, \cdots, a_k\}$�������������������һ�����У����ȡ�ߵ����Ȩֵ֮������Ƕ��١�ע�⣬�������ǽ����������һ�����У���˲��������ȡ���κ��򡣼�������ѯ��֮���Ƕ����ġ�

**�������ʽ��**

�ж���������ݡ���һ������һ������ $T$ ��ʾ������������������ÿ��������ݣ�

��һ�������������� $n$ �� $q$��$1 \leq n \leq 10^5$��$1 \leq q \leq 10^5$����ʾ���ӵ������Ͳ�����������

�ڶ������� $n$ ������ $c_1, c_2, \ldots, c_n$��$1 \leq c_i \leq n$�������� $c_i$ ��ʾ�� $i$ �����ӵĳ�ʼ��ɫ��

���������� $n$ ������ $v_1, v_2, \ldots, v_n$��$1 \leq v_i \leq 10^9$�������� $v_i$ ��ʾ�� $i$ �����������ĳ�ʼȨֵ��

���ڽ����� $q$ �У��� $i$ �������� $i$ �β�������ʽ���£�

- $1\; p\; x$����֤ $1 \leq p \leq n$ �� $1 \leq x \leq n$��
- $2\; p\; x$����֤ $1 \leq p \leq n$ �� $1 \leq x \leq 10^9$��
- $3\; x\; k\; a_1\; a_2\; \ldots \; a_k$����֤ $1 \leq x \leq n$ �� $1 \leq a_1 < a_2 < \ldots < a_k \leq n$ �� $c_x \in \{a_1, a_2, \cdots, a_k\}$��

��֤�������� $n$ ֮���� $q$ ֮�;������� $3 \times 10^5$������������ $k$ ֮�Ͳ����� $10^6$��

**�������ʽ��**

����ÿ�β��� $3$ ���һ��һ����������ʾȡ�ߵ����Ȩֵ֮�͵����ֵ��

```input1
2
5 10
1 2 3 1 2
1 10 100 1000 10000
3 3 1 3
3 3 2 2 3
2 5 20000
2 3 200
3 3 2 1 3
3 3 3 1 2 3
1 3 4
2 1 100000
1 2 2
3 1 2 1 2
4 1
1 2 3 4
1000000 1000000 1000000 1000000
3 4 4 1 2 3 4
```

```output1
100
110
1200
21211
100010
4000000
```

