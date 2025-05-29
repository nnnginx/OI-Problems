## ��Ŀ����
Misha needs to send packages to his friend Nadia. Both of them often travel across Russia, which is very large. So they decide to hire a messenger. Since the cost of the messenger service depends on the time it takes to deliver the package, they need your help to optimize a little bit.

Assume Misha and Nadia move on a two-dimensional plane, each visiting a sequence of places and moving along straight line segments from place to place. Your task is to find the shortest possible delivery time given their two paths.

Misha hands the package to the messenger at some point along his path. The messenger moves without delay along a straight line from the pick-up to intercept Nadia, who is traveling along her path. Misha, Nadia and the messenger move with a constant speed of $1$ distance unit per time unit. The delivery time is the time between Misha handing over the package and Nadia receiving it.

## �����ʽ
The input consists of a single test case. The test case contains two path descriptions, the first for Misha and the second for Nadia. Each path description starts with a line containing an integer $n$, the number of places visited ($2 \leq n \leq 50\, 000$). This is followed by $n$ lines, each with two integers $x_ i$ and $y_ i$ specifying the coordinates of a place ($0 \leq x_ i, y_ i \leq 30\, 000$). Coordinates of the places are listed in the order in which they are to be visited, and successive places do not have the same coordinates.

Misha and Nadia start their journeys at the same time, visiting the places along their paths without stopping. The length of each path is at most $10^6$. The package must be picked up at the latest when Misha reaches his final place and it must be delivered at the latest when Nadia reaches her final place.

## �����ʽ
Display the minimal time needed for delivery. Give the answer with an absolute error of at most $10^{-3}$ or a relative error of at most $10^{-5}$. If the package cannot be delivered, display impossible instead.

## ��Ŀ����
��Ŀ������  
ƽ�����������ƶ��ĵ� A,B������ A ��Ҫ�� B ����һ����Ϣ���������ͬʱ��������������һ�������ƶ����յ�Ϊֹ��A �����ƶ���;�з���һ����Ϣ��������Ϣ��������һ���� C��������һ�����������˶����� C �� B �غ�ʱ��B �����յ�����Ϣ��

A,B,C ���ƶ��ٶȶ��� 1 ��λ����ÿ�룬A �������������յ�ʱ������Ϣ��B ������Ҫ���������յ�ʱ�յ���Ϣ���� $t_A$ ��������Ϣ��ʱ�䣬$t_B$ ���������Ϣ��ʱ�䣬��ô����Ҫ��С�� $t_B-t_A$ ��ֵ���ر�أ���� B ������ζ��޷��յ���Ϣ������Ҫ��� `impossible`��

�����ʽ��

��һ�а���һ������ $n$������ A �������ߵĵ�����  
���� $n$ �У�ÿ�������������� $x_i,y_i$���������� A �������ߵĵ㡣  
����һ�а���һ������ $m$��B �����ߵĵ�����  
���� $m$ �У�ÿ�������������� $u_i,v_i$������ B �������ߡ�

�����ʽ��

һ�У����һ��ʵ��������𰸡����޷����㣬�����`impossible`��

```input1
2
0 0
0 10
2
4 10
4 0

```

```output1
4.00000

```

```input2
2
0 0
1 0
3
2 0
3 0
3 10

```

```output2
5.00000

```

## ��ʾ
Time limit: 3000 ms, Memory limit: 1048576 kB. 

 International Collegiate Programming Contest (ACM-ICPC) World Finals 2014

