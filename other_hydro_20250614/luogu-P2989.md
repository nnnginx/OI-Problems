## ��Ŀ����
Bessie is preparing her race car for the upcoming Grand Prix, but she wants to buy some extra parts to improve the car's performance. Her race car currently has mass M (1 <= M <= 1,000) and is able to push itself forward with a force of F (1 <= F <= 1,000,000). The Race Car Performance Store has N (1 <= N <= 10,000) parts

conveniently numbered 1..N. Bessie can buy as many or as few parts as she wishes though the store stocks no more than one instance of each part.

Part P\_i adds force F\_i (1 <= F\_i <= 1,000,000) and has mass

M\_i (1 <= M\_i <= 1,000). Newton's Second Law decrees that F =

MA, where F is force, M is mass, and A is acceleration. If Bessie wants to maximize the total acceleration of her race car (and

minimize the mass otherwise), which extra parts should she choose?

Consider a race car with initial F=1500 and M=100. Four parts are available for enhancement:

i  F\_i  M\_i

1  250   25

2  150    9

3  120    5

4  200    8

Adding just part 2, e.g., would result in an acceleration of

(1500+150)/(100+9) = 1650/109 = 15.13761. 

Below is a chart of showing the acceleration for all possible 

combinations of adding/not-adding the four parts (in column one, 1=part added, 0=part not added): 

Parts   Aggregate   Aggregate

1234        F           M       F/M

0000      1500         100    15.0000

0001      1700         108    15.7407

0010      1620         105    15.4286

0011      1820         113    16.1062

0100      1650         109    15.1376

0101      1850         117    15.8120

0110      1770         114    15.5263

0111      1970         122    16.1475 <-- highest F/M 

1000      1750         125    14.0000

1001      1950         133    14.6617

1010      1870         130    14.3846

1011      2070         138    15.0000

1100      1900         134    14.1791

1101      2100         142    14.7887

1110      2020         139    14.5324

1111      2220         147    15.1020

Thus, the best additional part combination is parts 2, 3, and 4.


## �����ʽ
\* Line 1: Three space-separated integers: F, M, and N

\* Lines 2..N+1: Line i+1 contains two space separated integers: F\_i and M\_i


## �����ʽ
\* Lines 1..P: The index values of P extra parts, one per line, that Bessie should add to her racecar. If she should not add any, output 'NONE' (without quotes). The output should be given in increasing order, so if the optimal set of parts is {2,4,6,7}, then the output should be in the order 2,4,6,7 and not, for example, 4,2,7,6. Solutions will be unique.


## ��Ŀ����
Bassie����Ϊ��������������������׼����

����һ����������ΪM���ҿ����ṩF������

��������Ҫ������������װһЩ������ܹ���N���������ÿ�������������$M_i$��$F_i$����ʾ�������Լ������ṩ������

��$X_i = 1\text{��}0$����ʾ��i�����ѡ��ѡ��

���$\frac{F+\sum_{i=1}^{n}X_i \times F_i}{M+\sum_{i=1}^{n}X_i \times M_i}$;

�ڴ˻�������С��$\sum_{i=1}^{n}X_i \times M_i + M$��

�����ʽ��

��һ���������ÿո�ֿ�����F,M,N

������N�У�ÿ��һ��������i+1�е�����������$F_i$��$M_i$

�����ʽ��

������յģ�����ԭʼ˳���ź���ķ���$\{i | X_i = 1\}$ ���ر�ģ���Bassie����Ҫ����������װ��������"None"��û��˫���ţ���

$N \le 10000 $

$M,M_i\le1000$

$F,F_i \le 1,000,000 $


��л@tyqtyq �ṩ�ķ���

```input1
1500 100 4 
250 25 
150 9 
120 5 
200 8 

```

```output1
2 
3 
4 

```

