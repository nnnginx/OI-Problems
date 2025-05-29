## ��Ŀ����
>$$������$$
>
>$$�����Ҳ������Ҫ���ȵ���\dots$$
>
>$$Ը�ҵĵ�����Ϩ�����ǵ�ʹ��\dots$$
>
>$$���������һλɢ���Ų�����Ϣ����ʹ��$$
>
>$$������ת������$$
>
>$$�Ҵ���û�����ǹ���\dots$$

## ��Ŀ����
���� $n,m$ �� $n$ ������ $a_i$��$1\le i\le n$����

��

$$ \sum\limits_{i=1}^{n} \sum\limits_{j=1}^{n}\left \lfloor \frac{m}{a_ia_j}  \right \rfloor$$

����𰸶� $998244353$ ȡģ�Ľ����

## �����ʽ
��һ������������ʾ $n,m$��

�ڶ��� $n$ ��������ʾ $a_1,a_2\dots a_n$��

## �����ʽ
һ��һ��������ʾ�𰸶� $998244353$ ȡģ��Ľ����

```input1
5 30
2 2 8 4 2 
```

```output1
88
```

```input2
10 5035239199
4853 53137 86933 4465 13588 11899 49877 16317 43326 52183 
```

```output2
2715
```

## ��ʾ
#### ���������͡�

����һ�еĹ������£�

$(a_1,a_1):\left \lfloor \frac{30}{2\times 2} \right \rfloor =7$��

$(a_1,a_2),(a_2,a_1):\left \lfloor \frac{30}{2\times 2} \right \rfloor \times 2=14$��

$(a_1,a_3),(a_3,a_1):\left \lfloor \frac{30}{2\times 8} \right \rfloor \times 2=2$��

$(a_1,a_4),(a_4,a_1):\left \lfloor \frac{30}{2\times 4} \right \rfloor \times 2=6$��

$(a_1,a_5),(a_5,a_1):\left \lfloor \frac{30}{2\times 2} \right \rfloor \times 2=14$��

$(a_2,a_2):\left \lfloor \frac{30}{2\times 2} \right \rfloor =7$��

$(a_2,a_3),(a_3,a_2):\left \lfloor \frac{30}{2\times 8} \right \rfloor \times 2=2$��

$(a_2,a_4),(a_4,a_2):\left \lfloor \frac{30}{2\times 4} \right \rfloor \times 2=6$��

$(a_2,a_5),(a_5,a_2):\left \lfloor \frac{30}{2\times 2} \right \rfloor \times 2=14$��

$(a_3,a_5),(a_5,a_3):\left \lfloor \frac{30}{2\times 8} \right \rfloor \times 2=2$��

$(a_4,a_4):\left \lfloor \frac{30}{4\times 4} \right \rfloor=1$��

$(a_4,a_5),(a_5,a_4):\left \lfloor \frac{30}{2\times 4} \right \rfloor \times 2=6$��

$(a_5,a_5):\left \lfloor \frac{30}{2\times 2} \right \rfloor=7$��

$7+14+2+6+14+7+2+6+14+2+1+6+7=88$��

#### �����ݷ�Χ��

| subtask ��� | $n$ | $m$ | $a_i$ | ��ֵ | �������� |
| :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| $0$ | $\le 10^2$ | $\le 10^{6}$ | $\le 10^5$ | $10$ | $-$ |
| $1$ | $\le 10^4$ | $\le 10^{10}$ | $\le 10^9$ | $10$ | $-$ |
| $2$ | $\le 10^6$ | $\le 10^{10}$ | $\le 10^4$ | $10$ | $-$ |
| $3$ | $\le 10^6$ | $\le 10^8$ | $\le 10^9$ | $20$ | $-$ |
| $4$ | $\le 10^6$ | $\le 10^{10}$ | $\le 10^9$ | $20$ | $A$ |
| $5$ | $\le 10^6$ | $\le 10^{10}$ | $\le 10^9$ | $30$ | $-$ |

�������� $A$��$\sum\limits_{i=1}^{n}a_i\le10^7$��

���� $100\%$ �����ݣ�$1\le n\le10^6$��$1\le a_i\le 10^9$��$\sum\limits_{i=1}^{n}a_i\le10^9$��$1\le m \le10^{10}$��

**�ر����ѣ�����ʹ�� subtask ������ԣ�ֻ��ͨ��һ���������ȫ�����Ե���ܻ�ô�������ķ�����**

