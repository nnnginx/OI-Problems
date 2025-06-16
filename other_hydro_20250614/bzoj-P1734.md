## ��Ŀ����

Farmer John has built a new long barn, with $n \ (2  \leq  n  \leq  10^5)$ stalls. The stalls are located along a straight line at positions $x_1,\dots ,x_n \ (0  \leq  x_i  \leq  10^9)$. His $c \ (2  \leq  c  \leq  n)$ cows don't like this barn layout and become aggressive towards each other once put into a stall. To prevent the cows from hurting each other, FJ want to assign the cows to the stalls, such that the minimum distance between any two of them is as large as possible. What is the largest minimum distance?

ũ�� John ������һ���ܳ��������������� $n$ �����䣬��ЩС�������α��Ϊ $x_1,\dots ,x_n$�����ǣ�John �� $c$ ͷţ�ǲ���ϲ�����ֲ��֣����Ҽ�ͷţ����һ����������Ǿ�Ҫ����������Ϊ�˲���ţ�����˺���John �����Լ���ţ������䣬ʹ������ͷţ֮�����С���뾡���ܵĴ���ô�����������С������ʲô�أ�

## �����ʽ

* Line $1$: Two space-separated integers: $n$ and $c$.
* Lines $2\dots n+1$: Line $i+1$ contains an integer stall location,$x_i$.

* ��һ�У��ո�ָ����������� $n$ �� $c$��
* �ڶ������� $n+1$ �У�$i+1$ ��ָ���� $x_i$ ��λ�á�

## �����ʽ

* Line $1$: One integer��the largest minimum distance.

* ��һ�У�һ��������������Сֵ��

```input1
5 3
1
2
8
4
9
```

```output1
3
```

## ����˵��

��ţ���� $1$��$4$��$8$ ������С������ $3$��

## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$2 \le n \le 10^5$��$0 \le x_i \le 10^9$��$2 \le c \le n$��
## ��Ŀ��Դ

Gold