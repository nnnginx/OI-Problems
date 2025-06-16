## ��Ŀ����
There are $n$ children playing with $n$ balls. Both children and balls are numbered from $1$ to $n$.

Before the game, $n$ integers $p_1, p_2, \cdots, p_n$ are given. In each round of the game, child $i$ will pass the ball he possesses to child $p_i$. It is guaranteed that no child will pass his ball to himself, which means $p_i \neq i$. Moreover, we also know that after each round, each child will hold exactly one ball.

Let $b_i$ be the ball possessed by child $i$. At the beginning of the game, child $i$ ($1 \le i \le n$) will be carrying ball $i$, which means $b_i=i$ initially. You're asked to process $q$ queries. For each query you're given an integer $k$ and you need to compute the value of $\sum\limits_{i=1}^{n} i \times b_i$ after $k$ rounds.

## �����ʽ
There is only one test case for each test file.

The first line of the input contains two integers $n$ ($2 \le n \le 10^5$) and $q$ ($1 \le q \le 10^5$), indicating the number of children and the number of queries.

The second line contains $n$ integers $p_1, p_2, \cdots, p_n$ ($1 \le p_i \le n$) indicating how the children pass the balls around.

For the following $q$ lines, the $i$-th line contains one integer $k_i$ ($1 \le k_i \le 10^9$) indicating a query asking for the result after $k_i$ rounds.

## �����ʽ
For each query output one line containing one integer indicating the answer.

## ��Ŀ����
**����Ŀ������**

�� $n$ �����Ӻ� $n$ ����������Ϸ�����Ӻ��򶼴� $1$ ��ŵ� $n$��

��Ϸ��ʼǰ�������� $n$ ������ $p_1, p_2, \cdots, p_n$������Ϸ��ÿһ���У����� $i$ �����������򴫸����� $p_i$����֤û�к��ӻ����������򴫸��Լ���Ҳ����˵ $p_i \neq i$�����⣬���ǻ�֪����ÿһ��֮��ÿ���������ﶼ�����ó���һ����

�� $b_i$ ��ʾ���� $i$ �����е�������Ϸ��ʼʱ������ $i$��$1 \le i \le n$����Я���� $i$��Ҳ����˵ $b_i=i$������Ҫ���� $q$ ����ѯ������ÿ����ѯ�����õ�һ������ $k$������Ҫ������ $k$ �ֺ� $\sum\limits_{i=1}^{n} i \times b_i$ ��ֵ��


**�������ʽ��**

����ĵ�һ�а����������� $n$��$2 \le n \le 10^5$���� $q$��$1 \le q \le 10^5$������ʾ���ӵ������Ͳ�ѯ��������

�ڶ��а��� $n$ ������ $p_1, p_2, \cdots, p_n$��$1 \le p_i \le n$������ʾ����֮�䴫��ķ�ʽ��

�������� $q$ ���У��� $i$ �а���һ������ $k_i$��$1 \le k_i \le 10^9$������ʾѯ���� $k_i$ �ֺ�Ľ����

**�������ʽ��**

����ÿ����ѯ�����һ�а���һ����������ʾ�𰸡�

**���������͡�**

ʾ�����������������¡�

$$
\begin{array}{|c|c|c|c|c|c|} \hline \textbf{�ִ�} & \textbf{b1} & \textbf{b2} & \textbf{b3} & \textbf{b4} & \textbf{��} \\\hline 
1 & 3 & 1 & 4 & 2 & 25 \\\hline
2 & 4 & 3 & 2 & 1 & 20 \\\hline
3 & 2 & 4 & 1 & 3 & 25 \\\hline
4 & 1 & 2 & 3 & 4 & 30 \\\hline
\end{array}
$$

���������ڣ�[ChatGPT](https://chatgpt.com/)��

```input1
4 4
2 4 1 3
1
2
3
4
```

```output1
25
20
25
30
```

## ��ʾ
The sample test case is explained below.

$$
\begin{array}{|c|c|c|c|c|c|} \hline \textbf{Round} & \textbf{b1} & \textbf{b2} & \textbf{b3} & \textbf{b4} & \textbf{Answer} \\\hline 
1 & 3 & 1 & 4 & 2 & 25 \\\hline
2 & 4 & 3 & 2 & 1 & 20 \\\hline
3 & 2 & 4 & 1 & 3 & 25 \\\hline
4 & 1 & 2 & 3 & 4 & 30 \\\hline
\end{array}
$$

