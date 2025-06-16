## ��Ŀ����
�����޸�ɸ�� Min_25 ɸ����Ҫǰ��֪ʶ��

## ��Ŀ����
�� $S(n)$ Ϊ $n$ ���������� $k$ �η��͡�

���� $N$��������ʽ�ӵ�ֵ��

$$\sum_{i=1}^{\lfloor\sqrt{N}\rfloor} i^2 S \!\left( \left\lfloor \frac{N}{i} \right\rfloor \right)$$

���н���Ը��������� $p$ ȡģ��



## �����ʽ
һ���������� $N,k,p$��֮���ÿո������

## �����ʽ
һ��һ���������������Ľ����

```input1
10 3 1000000007
```

```output1
1458
```

```input2
100000 0 1000000007
```

```output2
941229402
```

```input3
100000 10 1000000007
```

```output3
446053671
```

## ��ʾ
**��������** : 

$S \!\left( \left\lfloor \frac{N}{1} \right\rfloor \right)\! = S(10) = 2^3 + 3^3 + 5^3 + 7^3 = 503$��

$S \!\left( \left\lfloor \frac{N}{2} \right\rfloor \right)\! = S(5) = 2^3 + 3^3 + 5^3 = 160$��

$S \!\left( \left\lfloor \frac{N}{3} \right\rfloor \right)\! = S(3) = 2^3 + 3^3 = 35$��

$1^2 S \!\left( \left\lfloor \frac{N}{1} \right\rfloor \right)\! + 2^2 S \!\left( \left\lfloor \frac{N}{2} \right\rfloor \right)\! + 3^2 S \!\left( \left\lfloor \frac{N}{3} \right\rfloor \right)\! = 503 + 640 + 315 = 1458$��

| ���Ե��� | $N \le$ | $k \le$ | ʱ�� |
| :--: | :--: | :--: | :--: |
| $1\sim 3$ | $10^6$ | $10$ | $1\texttt s$ |
| $4\sim 7$ | $4\times {10}^{10}$ | $0$ | $3\texttt s$ |
| $8\sim 12$ | $4\times {10}^{10}$ | $10$ | $3\texttt s$ |

���� $100\%$ �����ݣ�$0 \le k \le 10$��$1 \le N \le 4\times {10}^{10}$��${10}^9 < p < 1.01 \times {10}^9$��

