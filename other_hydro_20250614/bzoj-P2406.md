## ��Ŀ����

����һ���������� $A[n\times m]$ ����һ������ $B[n\times m]$ ������ $\forall 1 \le i \le n , 1 \le j \le m , B_{i,j} \in [L,R]$ ����ʹ��ʽֵ��С��

$$
\max \left\{

\begin{aligned}

& \max\limits_{1 \le j \le m} \left\{ 

\begin{aligned}

\Bigg| \sum\limits_{i=1}^{n} (A_{i,j} - B_{i,j}) \Bigg|

\end{aligned}

\right\} \\

& \max\limits_{1 \le i \le n} \left\{ 

\begin{aligned}

\Bigg| \sum\limits_{j=1}^{m} (A_{i,j} - B_{i,j}) \Bigg|

\end{aligned}

\right\} \\

\end{aligned}

\right.
$$

## �����ʽ

��һ���������� $n , m$ ����ʾ����Ĵ�С��

������ $n$ �У�ÿ�� $m$ ���������������� $A$ ��

���һ������������ $L,R$ ��

## �����ʽ

���һ��һ����������𰸡�

```input1
2 2
0 1
2 1
0 1
```

```output1
1
```

## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ���֤ $n,m\le 200 , 0\le L\le R \le 1000 , 0 \le A_{i,j} \le 1000$ ��
