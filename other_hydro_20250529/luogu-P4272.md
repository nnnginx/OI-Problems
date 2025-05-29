## ��Ŀ����
����һ���������� $X_1, X_2, X_3, ... ,X_n$ ������������ $Q, A, B$ ���㣺

- $1 \leq X_i \leq Q$ �������� $1 \leq i \leq n$��

- $X_i \leq X_{i+1}$ �������� $1 \leq i < n$��

- $A \leq \frac{Q-1}{n-1}$ �� $A \leq B$��

�������� $1 \leq i \leq n$�������±任��$Y_i = X_i + \delta_i$������ $\delta_i$ ��һ��������ʹ�������� $Y$ �����������ʣ�

- $1 \leq Y_i \leq Q$ �������� $1 \leq i \leq n$��

- $Y_{i+1} - Y_i \in [A, B]$ �������� $1 \leq i < n$��

��������һ���任��������۶���Ϊ $\operatorname{TransformCost}(X, Y) = \sum_{i = 1}^{n}{\left\lvert\delta_i\right\rvert}$��

���������ΪѰ��һ���任��ʹ�� $\operatorname{TransformCost}(X, Y)$ ��С����


## �����ʽ
�����ļ� sequence.in �������С���һ�� $4$ ��������$N, Q, A, B$��������һ�а��� $N$ ���������ֱ�Ϊ $X_1, X_2, X_3, ... , X_n$��

## �����ʽ
����ļ� sequence.out ������һ�У�Ϊ��С�� $\operatorname{TransformCost}(X, Y)$��

```input1
3 6 2 2
1 4 6
```

```output1
1
```

## ��ʾ
### ����˵��

���Խ����б任Ϊ $2\ 4\ 6$ ���� $1\ 3\ 5$��ǰ�߱任����Ϊ $1$������Ϊ $2$�������С $\operatorname{TransformCost}$ Ϊ $1$��

### ���ݹ�ģ

���� $10\%$ ������ , $N \leq 100, Q \leq 10000, 1\leq A, B \leq 100$��

���� $30\%$ ������ , $N \leq 10000, Q \leq 10000, 1\leq A, B \leq 100$��

���� $60\%$ ������ , $N \leq 10000, Q \leq 10^9, 1\leq A, B \leq Q$��

���� $100\%$ ������, $N \leq 500000, Q \leq 10^9, 1\leq A, B \leq Q$��

