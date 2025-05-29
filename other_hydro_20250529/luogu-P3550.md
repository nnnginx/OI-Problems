## ��Ŀ����
Byteasar wants to take a taxi from the town Bytehole to the town Bytepit,    which is $m$ kilometres away from Bytehole.

Exactly $d$ kilometres along the way from Bytehole to Bytepit, there is    a base of $n$ taxis, numbered from $1$ to $n$.

The taxi no. $i$ has enough fuel to drive exactly $x_i$ kilometres.

Byteasar can change taxis at any point.

All the taxis start at their base but need not return there.

Your task is to determine whether Byteasar can be driven from Bytehole to    Bytepit, and if so, what it the minimum number of taxis required for such    a journey.

Translation 1:

һ���߶��������㣬0Ϊ��ʼλ�ã�dΪ���⳵�ܲ�λ�ã�mΪ�ҵ�λ�ã���Ҫ�г�����n���������ṩ��ÿ������һ��·�����ޣ����Ҷ��ӳ�վ�������еĳ���ʻ֮�󲻱���ص���վ�������ٽм�����

.Translation 2:

Byteasar�������⳵��Bytehole��Bytepit��,ǡ����dǧ�״�Bytehole��Bytepit��,����n�����⳵,��Ŵ�1��n.��i�����⳵���㹻��ȼ����ʻxiǧ��.Byteasar�����������ı���⳵.���еĳ��⳵�����ǵ��ܲ�������û��Ҫ�����ܲ�.����������ж�Byteasar�Ƿ��ܴ�Bytehole��Bytepit��,�������,���·;��Ҫ���⳵����С����.


## �����ʽ
The first line of the standard input holds three integers, $m$, $d$, and $n$ ($1\le d\le m\le 10^{18}$, $1\le n\le 500\ 000$),separated by single spaces.

Those denote, respectively: the distance from Bytehole to Bytepit,the distance from Bytehole to the taxi base, and the number of taxis at the base.

The second line of input contains $n$ integers, $x_1,x_2,\cdots,x_n$ ($1\le x_i\le 10^{18}$), separated by single spaces.

The number $x_i$ denotes the maximum distance (in kilometres) that the      i-th taxi can travel.

��һ�еı�׼������������ĸm,d,��n(1��d��m��1e18,1��n��500000)�м��ɿո����.

��Щ�ֱ��ʾ:��Bytehole��Bytepit��ľ���,��Bytehole�򵽳��⳵�ܲ��ľ���,�ܲ��ĳ��⳵����.

�ڶ����������n����ĸ;x1,x2...xn(1��xi��1e18),�м��ɿո����.

����xi��ʾ��i�����⳵����ʻ��������


## �����ʽ
Your program should print a single integer to the standard output:

the minimum number of taxis Byteasar has to take to get from Bytehole to Bytepit.  If getting there is impossible, your program should print the number $0$.

��ĳ���Ӧ�����һ������:��Ҫ����С�����ĳ��⳵����.������ܵ���,���0.


```input1
42 23 6
20 25 14 27 30 7

```

```output1
4

```

## ��ʾ
��ʾ:�����迪long long


