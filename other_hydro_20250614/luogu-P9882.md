## ��Ŀ����
Prof. Pang has an extraordinary vision. He can see the pixels on a 4K monitor. To test Prof. Pang's vision, Prof. Shou will show Prof. Pang several pixels and let Prof. Pang guess a straight line that contains these pixels. Given $k$ pixels with coordinates $(i, y_i)$ ($0\le i<k$), Prof. Pang must find nonnegative integers $a, b$ and $c$ (which represent the line $y=\frac{ax+b}{c}$) such that $y_i=\lfloor \frac{ai+b}{c} \rfloor$ for all $0\le i<k$. 

Prof. Shou will ask Prof. Pang multiple questions. They are given as follows: Prof. Shou has a fixed array $x_1,\ldots, x_n$. For each question, Prof. Shou chooses a range in the array, $x_l,\ldots, x_r$. Then he defines $y_i=x_{l+i}$ for $0\le i\le r - l$ and asks Prof. Pang to answer the question for the $r-l+1$ pixels $(0, y_0), \ldots, (r-l, y_{r-l})$.

Please help Prof. Pang answer all the questions. For each question, output the answer with the **minimum** $(c, a, b)$ **in lexical order**.

It is guaranteed that the answer exists when Prof. Pang chooses the whole array $x_1, x_2, \dots, x_n$. So the answer always exists when Prof. Pang chooses an interval of this array.

## �����ʽ
The first line contains a single integer $T$ ($1\le T\le 10^5$) denoting the number of test cases.

For each test case, the first line contains an integer $n$ ($1\leq n\leq 10^5$). The second line contains $n$ numbers $x_1, \ldots , x_{n}$ ($0\leq x_i\leq 10^9$).

The next line contains an integer $q$ ($1\le q\le 10^5$) denoting the number of questions.

Each of the following $q$ lines contains two integers $l, r$ ($1\le l\le r\le n$). 

It is guaranteed that the sum of $n$ over all test cases will not exceed $10^5$ and that the sum of $q$ over all test cases will not exceed $10^5$.

## �����ʽ
In the order of input, output one line with three integers $a, b, c$ denoting the answer for each question.

## ��Ŀ����
����һ������Ϊ $n$ ������ $x$������������ $q$ ��ѯ�ʡ�

�� $i$ ��ѯ�ʸ���һ������ $l,r$���� $k=r-l+1$������ȡ�� $x$ �����±��� $l,r$ ֮������� $y_i=x_{i+l}(0\le i<k)$��

���� $k$ ���� $(0,y_0),(1,y_1)\dots(k-1,y_{k-1})$������Ҫ�ҵ�һ��ֱ�ߵ������������� $a,b,c$������ $\forall 0\le i<k,y_i=\lfloor \frac{ai+b}{c}\rfloor$�����ж���������ֱ�ߣ���� $(c,a,b)$ ��Ԫ���ֵ�����С��һ����

��֤�����������飬�� $l=1,r=n$ ��ѯ��һ������һ��Ϸ��Ľ⡣

$n,q\le 10^5$������ѯ�ʡ�

```input1
3
5
1 1 2 2 2
4
1 5
1 1
3 5
2 3
5
1 2 3 4 6
3
1 5
2 4
3 5
3
0 3 5
1
1 3

```

```output1
1 4 3
0 1 1
0 2 1
1 1 1
5 4 4
1 2 1
3 6 2
5 1 2

```

