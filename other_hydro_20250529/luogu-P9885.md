## ��Ŀ����
Consider the following two sequences $P$ and $Q$. We denote $P(i)$ as the $i$-th element in sequence $P$, and $Q(i)$ as the $i$-th element in sequence $Q$:

- Sequence $P$ is a $\textbf{sorted}$ sequence where for all $k \in \mathbb{Z^+}$, $k$ appears in sequence $P$ for $(k+1)$ times ($\mathbb{Z^+}$ is the set of all positive integers). That is to say, $P = \{1, 1, 2, 2, 2, 3, 3, 3, 3, 4, 4, 4, 4, 4, 5, 5, 5, 5, 5, 5, 6, \dots \}$
- Sequence $Q$ can be derived from the following equations: 
$$\begin{cases} Q(1) = 1 & \\ Q(i) = Q(i-1) + Q(P(i)) & \text{if } i > 1 \end{cases}$$ 
That is to say, $Q = \{1, 2, 4, 6, 8, 12, 16, 20, 24, 30, 36, 42, 48, 54, 62, \dots \}$

![](https://cdn.luogu.com.cn/upload/image_hosting/ukq7qs74.png)

Given a positive integer $n$, please calculate the value of $Q(n)$.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ (about $10^4$), indicating the number of test cases. For each test case:

The first and only line contains an integer $n$ ($1 \le n \le 10^{40}$).

## �����ʽ
For each test case output one line containing one integer, indicating the value of $Q(n)$.

## ��Ŀ����
### ��Ŀ����  

���������������� $P$ �� $Q$�������� $P(i)$ ��ʾ���� $P$ �еĵ�  $i$ ��Ԫ�أ��� $Q(i)$ ��ʾ���� $Q$ �еĵ� $i$ ��Ԫ�أ�

- ���� $P$ ��һ��**�������**���У����У��������� $k \in \mathbb{Z^+}$��$k$ ������ $P$ �г��� $(k+1)$ �Σ�$\mathbb{Z^+}$ Ϊ������������Ҳ����˵��$P = \{1, 1, 2, 2, 2, 3, 3, 3, 3, 4, 4, 4, 4, 4, 5, 5, 5, 5, 5, 5, 6, \dots \}$
- ���� $Q$ ���������·��̵�����
$$\begin{cases} Q(1) = 1 & \\ Q(i) = Q(i-1) + Q(P(i)) & \text{if } i > 1 \end{cases}$$   
Ҳ����˵��$Q = \{1, 2, 4, 6, 8, 12, 16, 20, 24, 30, 36, 42, 48, 54, 62, \dots \}$��

![](https://cdn.luogu.com.cn/upload/image_hosting/ukq7qs74.png)

����һ�������� $n$������� $Q(n)$ ��ֵ��

### �����ʽ

����Ĳ��Ե��������������ݡ�

��һ���������һ������ $T$ ��$10^4$ ���ң�����ʾ�������ݵ�����������ÿ��������ݣ�

- ��һ�У�Ҳ��Ψһһ�У�����һ������ $n$ ��$1 \le n \le 10^{40}$����

### �����ʽ

����ÿ��������ݣ����һ�У�����һ����������ʾ $Q(n)$ ��ֵ��

```input1
4
10
100
1000
987654321123456789
```

```output1
30
2522
244274
235139898689017607381017686096176798
```

