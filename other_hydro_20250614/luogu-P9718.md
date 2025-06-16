## ��Ŀ����
Given a positive integer $x$, find the minimum positive integer $y$ such that the number of $\textbf{carries}^1$ of $x+y$ is exactly $k$.

We adds numbers $\textbf{by column addition in base-ten}$, just like what we normally do in primary school. For example, there are two carries in the following addition.

![](https://cdn.luogu.com.cn/upload/image_hosting/pfnper3r.png)

$^1$ which means ``��λ`` in Chinese.

## �����ʽ
The first line contains an integer $T$ $(1\leq T\leq 10^5)$ $-$ the number of test cases.

For each test case, the first line contains two integers $x, k$ $(1\leq x < 10^{18}, 0\leq k \leq 18)$.

## �����ʽ
For each test case, output one integer representing the answer in one line. If there is no solution, output $-1$ instead.

## ��Ŀ����
**����Ŀ������**

����һ�������� $x$���ҵ���С�������� $y$��ʹ�� $x+y$ �� $\textbf{��λ}$ ����ǡ��Ϊ $k$��

���ǰ���ʮ�����е��мӷ�������ӣ�����������Сѧʱ���������������磬����ļӷ��������ν�λ��

![](https://cdn.luogu.com.cn/upload/image_hosting/pfnper3r.png)

**�������ʽ��**

��һ�а���һ������ $T$ $(1\leq T\leq 10^5)$ $-$ ����������������

����ÿ��������������һ�а����������� $x, k$ $(1\leq x < 10^{18}, 0\leq k \leq 18)$��

**�������ʽ��**

����ÿ���������������һ��һ����������ʾ�𰸡����û�н������������� $-1$��

���������ڣ�[ChatGPT](https://chatgpt.com/)��

```input1
4
12345678 0
12345678 5
12345678 18
990099 5
```

```output1
1
54322
999999999987654322
9910
```

