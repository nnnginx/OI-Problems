## ��Ŀ����
����ַ��� $s$ ���㣺

- ����һ������ $(k,l)~(k\ge 1,l\ge 1)$��
- $s$ ���� $k$ ������Ϊ $l$ ���ַ��� $t$ ƴ�ӳɵġ�

��ô $s$ �ͱ�������һ�� $(k,l)\text{ - repeat}$ ����

�� $s=\tt abaabaabaaba$ ����һ�� $t=\tt aba$ �� $(4,3)\text{ - repeat}$ ����

����һ���ַ��� $u$�������ַ� $\texttt a$ �� $\texttt b$��������Ҫ�ҳ����е�һ���� $(k,l)\text{ - repeat}$ ����**������**�ַ�����ʹ $k$ �����ܴ�

���� $u=\tt babb\underline{abaabaabaaba}b$�����л��߲��־���һ�� $(4,3)\text{ - repeat}$ ������ʱ $k$ ��ֵ���

## �����ʽ
��һ��һ������ $n$������ $u$ �ĳ��ȡ�

������ $n$ �У�ÿ��һ���ַ���$\texttt a$ �� $\texttt b$������ʾ����ַ�����

## �����ʽ
��һ��һ���� $k$��

�ڶ���һ���� $l$��

������һ���� $p$����ʾ��� $(k,l)\text{ - repeat}$ ���Ŀ�ʼλ�ã�λ�ô� $1$ ��ʼ����

**����ж���������������һ�֡�**

```input1
17
b
a
b
b
a
b
a
a
b
a
a
b
a
a
b
a
b 
```

```output1
4
3
5
```

## ��ʾ
#### ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ��� $1\le n\le 5\times 10^{4}$��$u_i\in\{\tt a,b\}$��

#### ˵��

���� [BalticOI 2004 Day2 A REPEATS](https://boi.cses.fi/files/boi2004_day2.pdf)

�ر��л @[Sprague_Garundy](https://www.luogu.com.cn/user/764746) �ṩ�� SPJ��

