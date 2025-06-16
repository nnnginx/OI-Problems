## ��Ŀ����
![](https://cdn.luogu.com.cn/upload/image_hosting/g4ofcg40.png)

## ��Ŀ����
���Ԫ����� $k\operatorname A n$ Ϊ������ ${\rm A}_n^k$��$k \operatorname C n$ Ϊ����� ${\rm C}_n^k$������ $k>n$ ʱ���ߵ�ֵ��Ϊ $0$��

���� $n,m$ ��һ������Ϊ $n-1$ �Ľ����� $\textrm A,\textrm C$ ������ ${\rm opt}_{[1,n-1]}$�������г���Ϊ $n$����ÿһ�������� $[1,m]$ �е����������� $a_{[1,n]}$ �� $(\cdots(((a_1\operatorname{opt}_1 a_2)\operatorname{opt}_2 a_3)\operatorname{opt}_3 a_4)\cdots\operatorname{opt}_{n-2}a_{n-1})\operatorname{opt}_{n-1}a_n$ �ĺ͡�

�𰸶����� $11417603$ ȡģ��

## �����ʽ
��һ���������� $n,m$��

������һ��һ������Ϊ $n-1$ ���ַ�����ʾ $\text{opt}$��

## �����ʽ
һ��һ��������ʾ�𰸡�

```input1
2 2
C
```

```output1
4
```

```input2
2 2
A
```

```output2
5
```

```input3
8 8
CCACAAC
```

```output3
399968
```

## ��ʾ
#### ���������͡�
�������� #1��

$1\operatorname C 1=1$��$1\operatorname C 2=2$��$2\operatorname C 1=0$��$2\operatorname C 2=1$�����Ϊ $4$��

�������� #2��

$1\operatorname A 1=1$��$1\operatorname A 2=2$��$2\operatorname A 1=0$��$2\operatorname A 2=2$�����Ϊ $5$��

#### �����ݷ�Χ��

������������ԣ�������֡�

���� $100\%$ �����ݣ�$2\leq n,m\leq 10^5$��${\rm opt}$ ������ $\textrm A,\textrm C$��

| ���Ե��� | $n\leq$ | $m\leq$ | �������� |
| :----------: | :----------: | :----------: | :----------: |
| $1\sim3$ | $8$ | $8$ | �� | 
| $4\sim6$ | $314$ | $159$ | �� | 
| $7\sim10$ | $2718$ | $2818$ | �� | 
| $11\sim13$ | $10^5$ | $10^5$ | $\rm opt$ ���� $\rm A$ ���� |
| $14\sim16$ | $10^5$ | $10^5$ | $\rm opt$ ���� $\rm C$ ���� |
| $17\sim20$ | $10^5$ | $10^5$ | $\rm opt$ �ɲ����� $10$ �������� $\rm A$ �������� $\rm C$ ƴ�Ӷ��� |
| $21,22$ | $8492$ | $10^5$ | �� |
| $23\sim25$ | $10^5$ | $10^5$ | �� |

