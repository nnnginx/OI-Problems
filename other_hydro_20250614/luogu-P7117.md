## ��Ŀ����
����֮��������doge

## ��Ŀ����
��ǰ��һֻ Mivik����ϲ��������������������� $x$ �йصĶ���ʽ���� $f\left(x\right)$ �� $g\left(x\right)$ �� Mivik ������£�

$$
f\left(x\right)\otimes g\left(x\right)=\sum_{k=0}^{\deg f +\deg g}\max_{i\in [0,\deg f] \land j\in [0,\deg g]\land i+j=k}\left\{\left[x^i\right]f\left(x\right)+\left[x^j\right]g\left(x\right)\right\} x^k
$$

���� $\deg f$ ��ʾ $f$ ������������$\left[x^i\right]f\left(x\right)$ ���� $f\left(x\right)$ ��һ������ $x^i$ ��һ���ϵ����

��ע�⣬Mivik ��������ϵģ�Ҳ����˵ $a\otimes b\otimes c=(a\otimes b)\otimes c$��

Mivik ���� Mivik ����Ϊ�ܱ�ʾΪ $f\left(x\right)=ax+b$ ��ʽ�ĺ��������� $a$��$b$ ��Ϊ���������� $f\left(x\right)=-3+2x$ �� Mivik �������� $f\left(x\right)=\frac{1}{x}$ ���ǡ�

Mivik �ֶ���һ������ $f\left(x\right)$ �� simple �ģ����ҽ�������һ�� Mivik ���������� $S$����СΪ $\left|S\right|$����ʹ�ã�

$$
f\left(x\right)=S_1\otimes S_2\otimes S_3\otimes\cdots\otimes S_{\left|S\right|}.
$$

���� Mivik ������һ������ʽ������������������ǲ��� simple �ģ�����ǣ���˳�����������һ�ֿ��ܵ� $S$��

## �����ʽ
��һ��һ�������� $n$�������������ʽ������������

�ڶ��� $n$ �������������ӵ͵������δ����������ʽ������ϵ�� $f_i$����֤�����ϵ����Ϊ $0$��

## �����ʽ
�������������� simple �ģ����һ�� `nice`��

���������һ�� `simple`��Ȼ�������һ������㹹��� $S$ �Ĵ�С $\left|S\right|$���������� $\left|S\right|$ �и����㹹��� $S$ ���У�ÿ���������� $a$ �� $b$������һ�� Mivik ���� $f\left(x\right)=ax+b$��

```input1
3
2 3 3

```

```output1
simple
2
2 1
1 1

```

```input2
3
97 109 101

```

```output2
simple
2
54 42
47 55

```

```input3
9
9 9 8 2 4 4 3 5 3

```

```output3
nice

```

## ��ʾ
### �������� #1

�����ĺ��� $f\left(x\right)=2+3x+3x^2$ ������ $\left(2x+1\right)\otimes\left(x+1\right)$ �õ���

### ���Ե�Լ��

**�������������ԡ�**

����ȫ�����ݣ��� $1\le n\le 5\times 10^5$��$-10^8\le f_i\le 10^8$��

ÿ��������ľ������Ƽ��±�

| �������� | ��ֵ | $n\le$ |
|:-:|:-:|:-:|
| 1 | 5 | $1$ |
| 2 | 5 | $2$ |
| 3 | 20 | $20$ |
| 4 | 30 | $5000$ |
| 5 | 40 | $5\times 10^5$ |

**�������������ϴ���ʹ�ýϿ�Ķ��������ʽ��**

