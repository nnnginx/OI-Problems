## ��Ŀ����
A group of cows grabbed a truck and ventured on an expedition deep into the jungle. Being rather poor drivers, the cows unfortunately managed to run over a rock and puncture the truck's fuel tank. The truck now leaks one unit of fuel every unit of distance it travels. To repair the truck, the cows need to drive to the nearest town (no more than $10^6$ units distant) down a long, winding road. On this road, between the town and the current location of the truck, there are $n \ (1 \le  n \le  10^4)$ fuel stops where the cows can stop to acquire additional fuel ($1\dots 100$ units at each stop). The jungle is a dangerous place for humans and is especially dangerous for cows. Therefore, the cows want to make the minimum possible number of stops for fuel on the way to the town. Fortunately, the capacity of the fuel tank on their truck is so large that there is effectively no limit to the amount of fuel it can hold. The truck is currently L units away from the town and has $p$ units of fuel $\ (1 \le  p \le  10^6)$. Determine the minimum number of stops needed to reach the town, or if the cows cannot reach the town at all.

һȺ��ţ����һ����������ǰ��������̽�ա������������ǵļ�ʻ����̫�㣬������·�ϸ�Ū���ˣ���������ÿǰ��һ����λ��·�̾ͻ�©��һ����λ���ͣ�Ϊ���޺����䣬��ţ�Ǳ���ǰ������ĳ��У����ᳬ�� $10^6$ ��λ·�̣����ڵ�ǰλ�úͳ���֮���� $n$ ������վ����ţ�����ڼ���վ�� $1$ �� $100$ ��λ���͡���������˵�������Ǹ�Σ�յĵط�������ţ��˵���������������ԣ���ţҪ�����ܵ���ͣվ���͡����˵��ǣ���������������ǳ����������Ϊ���������������ġ���������� $p$ ����λʱ���� $l$ ����λ���͡���Ҫ�����ţ������Ҫͣ��վ���ܵ����У�������ţ�Ǹ��������˳��С�
## �����ʽ
* Line $1$: A single integer,$n$.
* Lines $2\dots n+1$: Each line contains two space-separated integers describing a fuel stop: The first integer is the distance from the town to the stop;the second is the amount of fuel available at that stop.
* Line $n+2$: Two space-separated integers, $l$ and $p$.
* ��һ�У�һ������ $n$��
* �ڶ��� $n+1$ �У�ÿ���������ÿո����������������һ������վ����һ������ʾ�������վ����еľ��룬�ڶ�������ʾ���������վ�����ԼӶ����͡�
* �� $n+1$ �У������ÿո�ֿ������� $l$ �� $p$��
## �����ʽ
* Line $1$: A single integer giving the minimum number of fuel stops necessary to reach the town. If it is not possible to reach the town, output `-1`.
* һ����ʾ��������������Ҫͣ�Ĵ���������޷�������� `-1`��

```input1
4
4 4
5 2
11 5
15 10
25 10
```

```output1
2
```
## ����˵��
INPUT DETAILS:  
The truck is $25$ units away from the town; the truck has $10$ units of fuel. Along the road, there are $4$ fuel stops at distances $4,5,11$, and $15$ from the town (so these are initially at distances $21,20,14$, and $10$ from the truck). These fuel stops can supply up to $4,2,5$, and $10$ units of fuel, respectively.

���ڿ�������� $25$ ����λ���������� $10$ ����λ���͡���·�ϣ��� $4$ ������վ���ֱ������� $4,5,11,15$���ֱ���뿨����Ϊ $21,20,14,10$. ��Щ����վ�ֱ����ɼ��� $4,2,5,10$ ����λ���� $10$ ����λ��
## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$1 \leq n \leq 10^4$��$1 \leq p \leq 10^6$��
## ��Ŀ��Դ
Gold