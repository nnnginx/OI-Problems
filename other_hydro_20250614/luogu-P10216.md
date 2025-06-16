## ��Ŀ����
��һ������Ϊ $2n$ ������ $\pi$ ������ƥ�䣬���ҽ���������
- $\forall 1\le i\le n,\pi_{2i-1}<\pi_{2i}$
- $\forall 1\le i< n,\pi_{2i-1}<\pi_{2i+1}$

�� $\textup{inv }\pi$ ��ʾ $\pi$ �����������$\textup{sgn }\pi=(-1)^{\textup{inv }\pi}$��$\mathfrak{M}_{2n}$ ��ʾȫ�峤��Ϊ $2n$ ������ƥ�乹�ɵļ��ϡ�
	
�� $\mathbf{A}=(a_{i,j})_{1\le i<j\le 2n}$ ��һ�����Գƾ��󣬶��� $\mathbf{A}$ �� $\text{Pfaffian}$ Ϊ
$$\textup{Pf}(\mathbf{A})=\sum\limits_{\pi\in\mathfrak{M}_{2n}}(\textup{sgn }\pi)\prod\limits_{i=1}^{n}a_{\pi(2i-1),\pi(2i)}$$

## ��Ŀ����
����ż�� $n$ �뷴�Գƾ��� $\mathbf{A}=(a_{i,j})_{1\le i<j\le n}$���� $\textup{Pf}(\mathbf{A})$ �� $10^9+7$ ȡģ�Ľ����

## �����ʽ
��һ��һ�������� $n$����֤ $n$ ��ż����

������ $n-1$ �У��� $i$ ���� $n-i$ ���Ǹ����������е� $j$ ��������ʾ $a_{i,i+j}$��

## �����ʽ
һ��һ���Ǹ���������ʾ�𰸡�

```input1
4
1 2 3
4 5
6
```

```output1
8
```

## ��ʾ
���� $30\%$ �����ݣ�$n\le 10$��

���� $100\%$ �����ݣ�$2\leq n\le 500$��$0\le a_{i,j}<10^9+7$��

