## ��Ŀ����
Farmer John has decided to take a cross-country vacation. Not wanting his cows to feel left out, however, he has decided to rent a large truck and to bring the cows with him as well!

The truck has a large tank that can hold up to G units of fuel (1 <= G <= 1,000,000).  Unfortunately, it gets very poor mileage: it consumes one unit of fuel for every unit of distance traveled, and FJ has a total of D units of distance to travel along his route (1 <= D <= 1,000,000,000).

Since FJ knows he will probably need to stop to refill his tank several times along his trip, he makes a list of all the N fuel stations along his route (1 <= N <= 50,000).  For each station i, he records its distance X\_i from the start of the route (0 <= X\_i <= D), as well as the price Y\_i per unit of fuel it sells (1 <= Y\_i <= 1,000,000).

Given this information, and the fact that FJ starts his journey with exactly B units of fuel (0 <= B <= D), please determine the minimum amount of money FJ will need to pay for fuel in order to reach his destination. If it is impossible for him to reach the destination, please output -1. Note that the answer to this problem may not fit into a standard 32-bit integer.


Farmer John ����ȥһ�ο�����ζȼ١�Ϊ�˲���������ţ�Ǹе�����������������һ���󿨳�����������ţ��һ�����С�


����������һ���ܴ�����䣬����װ�� $G$ ����λ���ͣ�$1 \le G \le {10}^6$�������ҵ��ǣ������ĺ�����Ҳ�ܴ󣬿���ÿ�˶�һ����λ�ľ��룬��Ҫ����һ����λ���͡�Farmer John Ҫ�������ó����� $D$ ����λ�ľ��롣��$1 \le D \le {10}^9$��


��Ϊ FJ ֱ��������Ҫ��������;��ͣ�£���������ͣ�������������;��·�ϵ� $N$ ������վ�ļ�¼�����˱�񡣶��ڵ� $i$ ������վ������¼�˼���վ�����ľ��� $X_i$��$0 \le X_i \le D$�����Լ�����վ��ÿ��λ�͵ļ۸� $Y_i$��$1 \le Y_i \le {10}^6$����

��֪������������Ϣ���Լ� FJ ��·;��ʼʱӵ�е�ȼ�͵����� $B$��$0 \le B \le D$���������� FJ ����Ŀ�ĵ�ʱ���ѵ��ͷ��õ���Сֵ����� FJ �޷�������;���յ㣬��ô����� `-1`������Ĵ𰸿����޷�ʹ�� 32 λ�������档


## �����ʽ
��һ�У� �ĸ�������$N, G, B, D$

������ $N$ �У�ÿһ�ж����������� $X_i$ �� $Y_i$��������������


## �����ʽ
һ����������� FJ �޷�������;���յ㣬��ô��� `-1`��������� FJ ����Ŀ�ĵ�ʱ���ѵ��ͷ��õ���Сֵ��


```input1
4 10 3 17
2 40
9 15
5 7
10 12
```

```output1
174

```

## ��ʾ
�������ͣ�FJ ���ƶ� $2$ ����λ��Ȼ��ͣ�¹��� $2$ ����λ���ͣ�Ҫ���� $40 \times 2$����Ȼ��һֱǰ����������� $5$ ����λ�ĵط�����ʱ����Ϊ�ա���ʱ������������ͣ�Ҫ���� $7 \times 10$��������ǰ�� $5$ ����λ���� $2$ ����λ���ͣ����� $12 \times 2$�������һֱ�ߵ��յ㡣��ʱ�ܻ����� $174$��


