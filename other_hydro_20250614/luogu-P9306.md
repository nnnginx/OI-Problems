## ��Ŀ����
**������ Maximum Version ��������������ֵ�����ݷ�Χ��ͬ��**

С L ��������������ʹ֮������

## ��Ŀ����
С L ��һ����Ϊ $n$ ������ $a$������ÿһ�� $a_i$ ����һ�� pair $(p_i, q_i)$��

Ϊ���� $a$ ����������һЩ�����ն� $p, q$ �ֱ��Ϊ��Ϊ $n$ �����С�

Ϊ�˶� $a$ �Ĺ����̶Ƚ����������㣬��������һ��Ȩֵ���� $f(a) = \displaystyle\sum_{i = 1}^n ([p_i > \max_{j = 1}^{i - 1} p_j] + [q_i > \max_{j = 1}^{i - 1} q_j])$��**ע�� $i = 1$ ʱ���������Ŷ���ȡ��ֵ����Ϊ������Ϊ $\displaystyle\max_{j = 1}^0 p_j = \displaystyle\max_{j = 1}^0 q_j = -\infty$��**

Ϊ���� $a$ ���������ӹ������������ֱ���ĳ�ַ�ʽ���� $a$ �õ� $a'$ ʹ�� $f(a')$ ��С��**ע������ʱ���뽫 $a'_i = (p'_i, q'_i)$ ��Ϊ���塣**

��ϣ������� $f(a')_{\min}$ ��ֵ���Լ��ֱ��ж��ٸ� $a'$ ����ȡ�� $f(a')_{\min}$��

���ڷ��������ܴܺ���ֻ��Ҫ�������� $998244353$ ȡģ��ֵ��

## �����ʽ
��һ�У�һ������ $n$��

�ڶ��У�$n$ ������ $p_1, p_2, \cdots, p_n$��

�����У�$n$ ������ $q_1, q_2, \cdots, q_n$��

## �����ʽ
һ�У�������������ʾ�����ֵ��

```input1
5
1 5 2 4 3
1 4 2 5 3
```

```output1
3 48
```

## ��ʾ
**�����ݷ�Χ��**

$$
\def\or{\operatorname{or}}
%\def\arrayscretch{1.5}
\def\arraystretch{1.5}
\begin{array}{|c|c|c|}\hline
\textbf{Subtask}&n\le &\textbf{Points}\cr\hline
\sf1&10&10 \operatorname{pts}\cr\hline
\sf2&500&20 \operatorname{pts}\cr\hline
\sf3&5\times10^3&20 \operatorname{pts}\cr\hline
\sf4&10^5&20 \operatorname{pts}\cr\hline
\sf5&5\times10^5&30 \operatorname{pts}\cr\hline
\end{array}
$$

���� $100\%$ �����ݣ�$1 \leq n \leq 5 \times 10^5$��$1 \leq p_i, q_i \leq n$����֤ $p, q$ ��Ϊ**����**��

