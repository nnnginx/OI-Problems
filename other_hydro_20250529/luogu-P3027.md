## ��Ŀ����
FJ�־�Ӫ���˹Ŷ����⣬����һЩ����ţʥ�����ϵ�װ��֮���С���⡣��֪�����Ὣ���ܴ洢��N(1<=N<=100)����ͬ����ţ�Ŷ�ÿ����������


�����������Ǯ�㹻��������������Ҫ�����������ĹŶ����������Թ���ĹŶ�����û�����ƣ�����ֻ��M(1<=M<=100,000)ԪǮ����Ŷ���������Ҫ�������̵ĵ�һ����ĩ��������������е����Խ��ͣ���


��i�ֹŶ��ɹ���Ҫ����Ci(1<=Ci<=100,000)ԪǮ��ÿ����һ�����Ի��Ri(1<=Ri<=100,000)ԪǮ(ÿ��һ��������ΪRi-Ci)��FJ����������˳���������Ļ����������Ҫ���������е�Ǯ������Ŷ���


FJ�������̵ĵ�һ����ĩ�ܵõ����������������=��ʼǮ��-�ܻ���+�����룩�Ƕ����أ��������ݱ�֤������ֲ��ᳬ��1,000,000,000.


����FJֻ��3�ֹŶ����ҿ�ʼʱ��M=17ԪǮ�����������ֹŶ��Ļ��Ѻ����롣


�Ŷ� ���� ����


1 2 4

2 5 6

3 3 7

����������£�FJӦ�û�15Ԫ����5��3�ŹŶ����ٻ�2Ԫ����1��1�ŹŶ����ܹ�17Ԫ������������5\*(7-3)+1\*(4-2)=5\*4+1\*2=22Ԫ�������ܻ�ñ������������ˡ�


��ʾ���ڶ�������������ս�ԣ������ǵĴ�����ȷ�ġ�


�����ʽ��


��1�У������Կո�ֿ���������N��M


��2�е���N+1�У���i+1�а��������Կո�ֿ���������Ci��Ri


�����ʽ


��1�У�FJ�ܻ�õ��������


## ��Ŀ����
FJ has gone into the curio business, buying and selling knickknacks like cow Christmas tree ornaments. He knows he will sell every single curio he can stock from a catalog of N (1 <= N <= 100)

different cow curios, and he can buy as many of each kind of curio as his heart desires. He has only M (1 <= M <= 100,000) money to invest but wants to maximize his profit (which has a slightly unusual definition) at the end of his first year in business.

Curio type i costs C\_i (1 <= C\_i <= 100,000) money to purchase and yields R\_i (1 <= R\_i <= 100,000) revenue for each curio sold (a profit of R\_i-C\_i). FJ can mix and match the curios he sells in any way he wishes. He need not spend all his money when purchasing curios.

What is the greatest amount of total profit (profit = initial\_cash - all\_costs + all\_sales) FJ can have at the end of his first year? This number is guaranteed to be less than 1,000,000,000.

Consider the situation when FJ has just 3 kinds of curios and starts with M=17. Below are the cost and revenue numbers for each curio:

Curio     Cost     Revenue

#        C\_i       R\_i

1         2         4

2         5         6

3         3         7

In this case, FJ should purchase 5 curios of type 3 for 15 money and 1 more curio of type 1 for 2 money, a total of 17 money. His profit will be 5 \* (7-3) + 1 \* (4-2) = 5\*4 + 1\*2 = 22 money. He can do no better than this given the cost and revenue structure.

NOTE: The second test case is challenging -- but our answer is correct.


## �����ʽ
\* Line 1: Two space-separated integers: N and M

\* Lines 2..N+1: Line i+1 contains two space-separated integers: C\_i and R\_i


## �����ʽ
\* Line 1: The maximum profit FJ can generate given the costs and revenues


```input1
3 17 
2 4 
5 6 
3 7 

```

```output1
22 

```

