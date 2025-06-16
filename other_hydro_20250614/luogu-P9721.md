## ��Ŀ����
$\textbf{This is an interactive problem.}$

There is a hidden permutation $p_1, p_2, \dots, p_n$ of $\{1, 2, \dots, n\}$. You want to find it by asking the parity of the number of inversions of $p_l,\ldots, p_r$.

You can query in the format ${?~l~r}$, and the interactor will respond you $\left( \sum_{l\leq i < j\leq r} [p_i > p_j]\right) \bmod 2$. $[p_i>p_j]$ is $1$ when $p_i>p_j$ and $0$ when $p_i\le p_j$.

## �����ʽ
Firstly, you should read the integer $n$ ($1\le n\le 2000$).

After that, you can make no more than $4 \times 10^4$ queries. To make a query, output ``${?~l~r}$'' ($1 \leq l \leq r \leq n$) on a separate line, then you should read the response from standard input. 

To give your answer, print ``${!~p_1~p_2~\dots~p_n}$'' on a separate line. The output of the answer is \textbf{not} counted towards the limit of $4 \times 10^4$ queries. 

After that, your program should terminate. 

After printing a query, do not forget to output end of line and flush the output. To do this, use $\texttt{fflush(stdout)}$ or $\texttt{cout.flush()}$ in C++, $\texttt{System.out.flush()}$ in Java, $\texttt{flush(output)}$ in Pascal, or $\texttt{stdout.flush()}$ in Python. 

It is guaranteed that the permutation is fixed in advance. 

## ��Ŀ����
**����Ŀ������**

����һ������ʽ���⡣

��һ�����ص����� $p_1, p_2, \dots, p_n$�����а��� $\{1, 2, \dots, n\}$ �����С�����ͨ��ѯ�� $p_l,\ldots, p_r$ ���������������ż�����ҵ�����

������� ${?~l~r}$ �ĸ�ʽ���в�ѯ����������ش��� $\left( \sum_{l\leq i < j\leq r} [p_i > p_j]\right) \bmod 2$������ $[p_i>p_j]$ �� $p_i>p_j$ ʱΪ $1$���� $p_i\le p_j$ ʱΪ $0$��

���ȣ�����Ҫ�������� $n$��$1\le n\le 2000$����

֮������Խ��в����� $4 \times 10^4$ �β�ѯ��Ҫ���в�ѯ����� ${?~l~r}$��$1 \leq l \leq r \leq n$���ڵ�����һ���ϣ�Ȼ����Ӧ�ôӱ�׼�����ж�ȡ��Ӧ��

Ҫ������Ĵ𰸣��� ${!~p_1~p_2~\dots~p_n}$ ��ӡ�ڵ�����һ���ϡ��𰸵���� $\textbf{��}$ ���� $4 \times 10^4$ �β�ѯ�����ơ�

֮����ĳ���Ӧ����ֹ��

�ڴ�ӡ��ѯ�󣬲�Ҫ����������в�ˢ�������Ҫ������һ�㣬�� C++ ��ʹ�� $\texttt{fflush(stdout)}$ �� $\texttt{cout.flush()}$���� Java ��ʹ�� $\texttt{System.out.flush()}$���� Pascal ��ʹ�� $\texttt{flush(output)}$�������� Python ��ʹ�� $\texttt{stdout.flush()}$��

��֤������ǰ�̶���

���������ڣ�[ChatGPT](https://chatgpt.com/)

```input1
3

0

0

1

```

```output1

? 1 2

? 1 3

? 2 3

! 2 3 1
```

