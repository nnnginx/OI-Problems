## ��Ŀ����

�� $n$ ��ש��Ҫ��һ�� $n$ �������Ҫ�����ש $a$ ��ש $b$ ���棬��ô $a$ ���ܱ� $b$ �ĳ��� $+ d$ Ҫ�������м��ַ���������� $\bmod\ 10^9+9$ ��ֵ��

## �����ʽ

��һ�У�$n,d$��

�ڶ��У�$n$ ��������ʾÿ��ש�ĳ��ȡ�

## �����ʽ

�����������Ҫ $\bmod\ 10^9+9$��

```input1
4 1
1 2 3 100
```
```output1
4
```

## ����˵�� 1

We can arrange the first three blocks in any order, except for $2,1,3$ or $1,3,2$. The last block has to be at the bottom.

```input2
6 9
10 20 20 10 10 20
```
```output2
36
```

## ����˵�� 2

We are not allowed to put a cube of size $20$ onto a cube of size $10$.

There are six ways to order the cubes of size $10$, and six ways to order the cubes of size $20$.

## ���ݹ�ģ��Լ��

���� $10\%$ �����ݣ�$n \leq 10$��

���� $30\%$ �����ݣ������������� $10^6$��

���� $45\%$ �����ݣ�$n \leq 20$��

���� $70\%$ �����ݣ�$n \leq 70$��

���� $100\%$ �����ݣ�$ 2 \leq n \leq 6.2\times 10^5$����������������Ϊ������ $10^9$ ����������