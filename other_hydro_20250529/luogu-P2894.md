## ��Ŀ����
The cows are journeying north to Thunder Bay in Canada to gain cultural enrichment and enjoy a vacation on the sunny shores of Lake Superior. Bessie, ever the competent travel agent, has named the Bullmoose Hotel on famed Cumberland Street as their vacation residence. This immense hotel has N (1 �� N �� 50,000) rooms all located on the same side of an extremely long hallway (all the better to see the lake, of course).

The cows and other visitors arrive in groups of size Di (1 �� Di �� N) and approach the front desk to check in. Each group i requests a set of Di contiguous rooms from Canmuu, the moose staffing the counter. He assigns them some set of consecutive room numbers r..r+Di-1 if they are available or, if no contiguous set of rooms is available, politely suggests alternate lodging. Canmuu always chooses the value of r to be the smallest possible.

Visitors also depart the hotel from groups of contiguous rooms. Checkout i has the parameters Xi and Di which specify the vacating of rooms Xi ..Xi +Di-1 (1 �� Xi �� N-Di+1). Some (or all) of those rooms might be empty before the checkout.

Your job is to assist Canmuu by processing M (1 �� M < 50,000) checkin/checkout requests. The hotel is initially unoccupied.

��һ������ $n,m$��$n$ ������ $n$ ������ $(1\leq n \leq 50,000)$�����Ϊ $1 \sim n$����ʼ��Ϊ�շ���$m$ ��ʾ������ $m$ �в��� $(1\leq m < 50,000)$������ÿ��������һ���� $i$ ����ʾһ�ֲ�����

�� $i$ Ϊ $1$����ʾ��ѯ���䣬������һ���� $x$����ʾ�� $1,2,...,n$ �������ҵ�����Ϊ $x$ �������շ���������� $x$ ����������˵ķ���ţ�����������������С�����Ҳ�������Ϊ $x$ �������շ������ $0$�����ҵõ������� $x$ ���շ�����ס���ˡ�

�� $i$ Ϊ $2$����ʾ�˷��������������� $x,y$ ������� $x \sim x+y-1$ �˷������÷���Ϊ�ա�

����Ҫ��ÿ������ $1$ �����Ӧ�Ĵ𰸡�

## �����ʽ
\* Line 1: Two space-separated integers: N and M

\* Lines 2..M+1: Line i+1 contains request expressed as one of two possible formats: (a) Two space separated integers representing a check-in request: 1 and Di (b) Three space-separated integers representing a check-out: 2, Xi, and Di


## �����ʽ
\* Lines 1.....: For each check-in request, output a single line with a single integer r, the first room in the contiguous sequence of rooms to be occupied. If the request cannot be satisfied, output 0.


```input1
10 6
1 3
1 3
1 3
1 3
2 5 5
1 6

```

```output1
1
4
7
0
5

```

