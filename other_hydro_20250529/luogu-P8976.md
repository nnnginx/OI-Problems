## ��Ŀ����
**Update on 2023.2.1������һ����� @[yuanjiabao](https://www.luogu.com.cn/user/455558) �� Hack ���ݣ������� #21��**

**Update on 2023.2.2������һ����� @[CourtesyWei](https://www.luogu.com.cn/user/664070) �� @[bizhidaojiaosha](https://www.luogu.com.cn/user/613616) �� Hack ���ݣ������� #22��**

------------

~~����һ������ $p$��ʹ��~~$\small\color{white}{�±�Ϊ��������֮�� \geq a ���±�Ϊż������֮�� \geq b��}$

## ��Ŀ����
С L ����һ��**ż��** $n$ ���������� $a, b$�����㹹��һ����Ϊ $n$ ������ $p$��ʹ�������� $\displaystyle\sum_{i = 1}^{\frac{n}{2}} p_i \geq a$ �� $\displaystyle\sum_{i = \frac{n}{2} + 1}^{n} p_i \geq b$��

## �����ʽ
**�����ж���������ݡ�**

��һ�У�һ������ $T$����ʾ����������

����ÿ�����ݣ�

һ�У��������� $n, a, b$��

## �����ʽ
����ÿ�����ݣ�����޽⣬��� $-1$���������һ�У�$n$ ����������ʾ�㹹��������� $p$��

**���ж�⣬�������һ����ɡ�**

```input1
2
6 6 12
6 8 14
```

```output1
1 6 2 5 3 4
-1
```

## ��ʾ
**���⿪�� Special Judge��**

| $\textbf{Subtask}$ | $n$ | $a, b$ | ��ֵ |
| :------: | :------: | :------: | :------: |
| $1$ | $2 \leq n \leq 10$ | ���������� | $20 \operatorname{pts}$ |
| $2$ | ���������� | $a = b = 0$ | $10 \operatorname{pts}$ |
| $3$ | ͬ�� | $a = 0$ �� $b = 0$ | $10 \operatorname{pts}$ |
| $4$ | ͬ�� | ���������� | $60 \operatorname{pts}$ |

���� $100\%$ �����ݣ�$2 \leq n, \sum n \leq 10^5$��$0 \leq a, b \leq \frac{n(n + 1)}{2}$��$1 \leq T \leq 10$��$n$ Ϊ**ż��**��

