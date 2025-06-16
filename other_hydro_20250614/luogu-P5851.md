## ��Ŀ����
Farmer John has $M$ cows, conveniently labeled $1 \ldots M$, who enjoy the occasional change of pace
from eating grass.  As a treat for the cows, Farmer John has baked $N$ pies ($1 \leq N \leq 300$), labeled
$1 \ldots N$.  Cow $i$ enjoys pies with labels in the range $[l_i, r_i]$ (from $l_i$ to $r_i$ inclusive),
and no two cows enjoy the exact same range of pies.  Cow $i$ also has a weight, $w_i$, which 
is an integer in the range $1 \ldots 10^6$.

Farmer John may choose a sequence of cows $c_1,c_2,\ldots, c_K,$ after which the
selected cows will take turns eating in that order. Unfortunately, the cows 
don't know how to share! When it is cow $c_i$'s turn to eat, she will consume
all of the  pies that she enjoys --- that is, all remaining pies in the interval
$[l_{c_i},r_{c_i}]$.  Farmer John would like to avoid the awkward situation
occurring when it is a cows turn to eat but all of the pies she enjoys have already been
consumed. Therefore, he wants you to compute the largest possible total weight
($w_{c_1}+w_{c_2}+\ldots+w_{c_K}$) of a sequence $c_1,c_2,\ldots, c_K$ for which each cow in the
sequence eats at least one pie.

## ��Ŀ����
Farmer John �� $M$ ͷ��ţ��Ϊ�˷��㣬���Ϊ $1,\dots,M$����Щ��ţƽʱ������ݣ�����ϲ��ż��������ζ��Farmer John һ�쿾�� $N$ ��������ţ�ԣ��� $N$ ���ɱ��Ϊ $1,\dots,N$���� $i$ ͷ��ţϲ���Ա���� $\left[ l_i,r_i \right]$ �е��ɣ��������ˣ�������û����ͷ��ţϲ������ͬ��Χ���ɡ��� $i$ ͷ��ţ��һ������ $w_i$������һ���� $\left[ 1,10^6 \right]$ �е���������

Farmer John ����ѡ��һ����ţ���� $c_1,c_2,\dots,c_K$��������Щ��ţ�����˳���������ɡ����ҵ��ǣ���Щ��ţ��֪����������ţ  ����ʱ���������ϲ���Ե��ɶ��Ե�����Ҳ����˵������Ե������ $[l_{c_i},r_{c_i}]$ ������ʣ����ɡ�Farmer John ��Ҫ���⵱�ֵ�һͷ��ţ����ʱ��������ϲ��������֮ǰ�����Ե����������ε��������ˣ�����������㣬Ҫʹ��ţ�� $c_1,c_2,\dots,c_K$ ��˳����ɣ��ֵ���ͷ��ţʱ��ϲ����������ʣ��һ��������£���Щ��ţ�����������أ�$w_{c_1}+w_{c_2}+\ldots+w_{c_K}$���Ƕ��١�

## �����ʽ
��һ�а������������� $N,M$��

������ $M$ �У�ÿ������������ $w_i,l_i,r_i$��

## �����ʽ
�������һ���Ϸ������У������ܵ�����ֵ��

```input1
2 2
100 1 2
100 1 1

```

```output1
200

```

## ��ʾ
#### ��������
����������У������ţ $1$ �ȳԣ���ô��ţ $2$ �ͳԲ������ˡ�Ȼ����������ţ $2$ �ԣ�Ȼ����ţ $1$ ֻ�Ա��Ϊ $2$ ���ɣ��Կ�������������

����ȫ�����ݣ�$1 \le N \le 300,1 \le M \le \dfrac{N(N-1)}{2},1 \le l_i,r_i \le N,1 \le w_i \le 10^6$��
#### ���ݷ�Χ
���ڲ��Ե� $2-5$������ $N \le 50,M \le 20$��

���ڲ��Ե� $6-9$������ $N \le 50$��

USACO 2019 December ������T1

