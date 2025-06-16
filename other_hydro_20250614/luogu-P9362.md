## ��Ŀ����
We define a function $f(x)$ over all non-negative integer $x$ as follows:
$$
f(x) =
\begin{cases}
1 & (x = 0) \\
f(\frac{x}{3}) + 1 & (x > 0\land x\bmod3 = 0) \\
f(x - 1) + 1  & (x > 0\land x\bmod 3\neq 0)
\end{cases}
$$
Calculate $\max_{x = l} ^ r f(x)$.

You need to answer $T$ queries independently.

## �����ʽ
The first line contains a single integer $T$ ($1\leq T\leq 10 ^ 4$).

Each of the next $T$ lines contains two integers $l$ and $r$ ($1\leq l\leq r\leq 10 ^ {18}$), representing a query.

## �����ʽ
Output $T$ lines. The $i$-th line contains a single integer, representing the answer to the $i$-th query.

## ��Ŀ����
### ��Ŀ����

���������зǸ����� $x$ �ϵĺ��� $f(x)$ ���£�

$$
f(x) =
\begin{cases}
1 & (x = 0) \\
f(\frac{x}{3}) + 1 & (x > 0\land x\bmod3 = 0) \\
f(x - 1) + 1  & (x > 0\land x\bmod 3\neq 0)
\end{cases}
$$

���� $\max_{x = l} ^ r f(x)$��

���� $T$ �����ݡ�

$1\leq T\leq 10 ^ 4$��$1\leq l\leq r\leq 10 ^ {18}$��

### �����ʽ

��һ��һ������ $T$��

������ $T$ �У�ÿ���������� $l, r$ ��ʾһ��ѯ�ʡ�

### �����ʽ

����ÿ��ѯ�ʣ����һ��һ��������ʾ�𰸡�



```input1
10
1 2
1 3
1 4
1 5
2 3
2 4
2 5
3 4
3 5
4 5

```

```output1
3
3
4
5
3
4
5
4
5
5

```

## ��ʾ
**Source**: The 2022 ICPC Asia Xi'an Regional Contest Problem E.

**Author**: MagicSpark.

