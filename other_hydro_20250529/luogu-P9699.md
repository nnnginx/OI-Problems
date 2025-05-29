## ��Ŀ����
For positive integers $X$ and $b \geq 2$, define $f(X,b)$ as a sequence which describes the base-$b$ representation of $X$, where the $i$-th element in the sequence is the $i$-th least significant digit in the base-$b$ representation of $X$. For example, $f(6, 2) = \{0, 1, 1\}$, while $f(233, 17) = \{12, 13\}$.

Given four positive integers $x$, $y$, $A$ and $B$, please find two positive integers $a$ and $b$ satisfying:

- $2 \leq a \leq A$
- $2 \leq b \leq B$
- $f(x, a) = f(y, b)$

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ ($1 \leq T \leq 10^3$) indicating the number of test cases. For each test case:

The first line contains four integers $x$, $y$, $A$ and $B$ ($1 \leq x,y \leq 10^9$, $2 \leq A,B \leq 10^9$).

It's guaranteed that there are at most $50$ test cases satisfying $\max(x, y) > 10^6$.

## �����ʽ
For each test case, if valid positive integers $a$ and $b$ do not exist, output $\texttt{NO}$ in one line.

Otherwise, first output $\texttt{YES}$ in one line. Then in the next line, output two integers $a$ and $b$ separated by a space. If there are multiple valid answers, you can output any of them.

## ��Ŀ����
**����Ŀ������**

���������� $X$ �� $b \geq 2$������ $f(X,b)$ Ϊһ�������� $X$ �� $b$ ���Ʊ�ʾ�µ����У��������еĵ� $i$ ��Ԫ�ر�ʾ $X$ �� $b$ ���Ʊ�ʾ�´ӵ͵��ߵ� $i$ λ��ֵ�����磬$f(6, 2) = \{0, 1, 1\}$���� $f(233, 17) = \{12, 13\}$��

�������ĸ������� $x$��$y$��$A$ �� $B$�����ҵ����������� $a$ �� $b$��ͬʱ���㣺

- $2 \leq a \leq A$
- $2 \leq b \leq B$
- $f(x, a) = f(y, b)$

**�������ʽ��**

�ж���������ݡ���һ������һ������ $T$��$1 \leq T \leq 10^3$����ʾ������������������ÿ��������ݣ�

��һ�������ĸ����� $x$��$y$��$A$ �� $B$��$1 \leq x,y \leq 10^9$��$2 \leq A,B \leq 10^9$����

��֤����ֻ�� $50$ ������������� $\max(x, y) > 10^6$��

**�������ʽ��**

����ÿ��������ݣ���������ںϷ��������� $a$ �� $b$�������һ��һ���ַ��� $\texttt{NO}$��

�����������һ��һ���ַ��� $\texttt{YES}$����һ����������ɵ����ո�ָ������� $a$ �� $b$������ж��ֺϷ��𰸣��������������һ�֡�

```input1
6
1 1 1000 1000
1 2 1000 1000
3 11 1000 1000
157 291 5 6
157 291 3 6
10126 114514 789 12345
```

```output1
YES
2 2
NO
YES
2 10
YES
4 5
NO
YES
779 9478
```

