## ��Ŀ����
Once again, Xingqiu hides Chongyun's ice cream into a box with a strange lock. Liyue's summer has been always very hot and Chongyun suffers more because of his excessive yang (positive) energy, so he needs that ice cream desperately.

![](https://cdn.luogu.com.cn/upload/image_hosting/2dtcr426.png)

There are two integers $a$ and $b$ on the lock. Chongyun can perform the following three types of operations any number of times:
- Minus $1$ from both $a$ and $b$;
- Plus $1$ to both $a$ and $b$;
- Divide both $a$ and $b$ by one of their common $\textbf{prime}$ factor (that is to say, divide them by a $\textbf{prime}$ $g$ where $a$ and $b$ are both divisible by $g$).

The box will be unlocked if either $a$ or $b$ or both become $1$. To help Chongyun gets the ice cream back as quickly as possible, please tell him the minimum number of operations needed to unlock the box.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ ($1 \le T \le 300$) indicating the number of test cases. For each test case:

The first and only line contains two integers $a$ and $b$ ($1 \le a, b \le 10^9$, $a \ne b$).

## �����ʽ
For each test case output one line containing one integer indicating the minimum number of operations to make $a$ or $b$ or both equal $1$.

## ��Ŀ����
## ��Ŀ����
�� $T$ �����ӣ�ÿ��������һ�������������������� $a$ �� $b$������Զ�����������ɴ����� 3 �ֲ�����

- $a$ �� $b$ �ֱ��ȥ $1$
- $a$ �� $b$ �ֱ����� $1$
- $a$ �� $b$ �ֱ�������ǹ�ͬ����������

��� $a$ �� $b$ �����߶���Ϊ $1$�����Ӿͻ�����������дһ�����򣬼���ÿ�����ӵ����򿪵����ٲ���������

## �����ʽ
��һ������һ������ $T(1��T��300)$��

������ $T$ �У�ÿ������ $a$ �� $b$����ʾÿ�����ӵ�������Ϣ��

## �����ʽ  

����� $T$ �У�ÿ�������Ӧ���ӽ��������ٲ��衣

```input1
5
4 7
9 8
32 84
11 35
2 1

```

```output1
2
7
5
4
0

```

## ��ʾ
For the first sample test case, the optimal way is $(4, 7) \rightarrow (3, 6) \rightarrow (1, 2)$.

For the second sample test case, the optimal way is to apply the first type of operation $7$ times.

For the third sample test case, the optimal way is $(32, 84) \rightarrow (16, 42) \rightarrow (15, 41) \rightarrow (14, 40) \rightarrow (13, 39) \rightarrow (1, 3)$.

For the fourth sample test case, the optimal way is $(11, 35) \rightarrow (12, 36) \rightarrow (6, 18) \rightarrow (2, 6) \rightarrow (1, 3)$.

