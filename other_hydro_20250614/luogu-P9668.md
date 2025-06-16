## ��Ŀ����
Prof. Pang and Prof. Shou go to explore a cave together. Prof. Pang walks ahead of Prof. Shou. 

Each of them has a torch for illumination. The torches need fuel to burn. Prof. Pang's torch can burn for $a_1$ seconds once it has been refilled, and it takes $b_1$ seconds to refuel the torch after it burns out. Prof. Shou's torch can burn for $a_2$ seconds once it has been refilled, and it takes $b_2$ seconds to refuel the torch after it burns out. The person who is refueling the torch cannot walk simultaneously. For safety reasons, they cannot refuel the torch until the fuel runs out. 

Because Prof. Pang is too fat and the cave is too narrow, Prof. Shou cannot surpass Prof. Pang during the exploration, which means that Prof. Shou is at least 1 unit behind Prof. Pang. 

Each of them can walk forward a distance of 1 unit per second when his torch is burning. Every second, Prof. Pang moves first, then Prof. Shou does. In order to get to their destination earlier, they will move as long as they can walk forward. 

Now Prof. Shou has $n$ questions, and for the $i$-th question, he wants to know that at time $q_i$, how many units of the distance he has moved forward from the starting point? Prof. Shou starts 1 unit behind Prof. Pang. The initial time is 0. Both Prof. Pang and Prof. Shou refueled the torch before the initial time.

## �����ʽ
The first line contains one integer $T~(1\le T \le 10^5)$, the number of test cases.

For each test case, the first line contains 5 integers $a_1, b_1, a_2, b_2, n~(1 \le a_1, b_1, a_2, b_2, n \le 10^6)$ denoting the time Prof. Pang's torch can burn, the time for Prof. Pang to refuel his torch, the time Prof. Shou's torch can burn, the time for Prof. Shou to refuel his torch, and the number of Prof. Shou's queries. Each of the next $n$ lines describes a query. Query $i$ is denoted by one integer $q_i~(1 \le q_i \le 10^{16})$.

It is guaranteed that over all test cases, each of the following numbers is no more than $10^6$:

- the sum of $a_1$, 
- the sum of $a_2$, 
- the sum of $b_1$, 
- the sum of $b_2$, 
- and the sum of $n$.

## �����ʽ
For each query, print one line containing the answer -- the number of units that Prof. Shou has walked forward from the starting point.

## ��Ŀ����
## ��Ŀ����

���Ӻ�������һ��ɽ�������ߣ�����������ǰ�档ÿ���˶���һ֧��ѡ�

���ӵĻ������ȼ�Ϻ����ȼ�� $a_1$ �룬��Ϩ�����Ҫ���� $b_1$ �����ȼ�ϡ�

���ӵĻ������ȼ�Ϻ����ȼ�� $a_2$ �룬��Ϩ�����Ҫ���� $b_2$ �����ȼ�ϡ�

ÿ����ֻ�����Լ��Ļ��ȼ��ʱǰ�����ٶ�Ϊ $1\operatorname{m/s}$��

��Ϊ����̫�֣���������ֻ�ܸ������Ӻ�������ܳ������ӡ�

ÿһ���������ƶ���֮���������ƶ���

��ʼʱ�����˵Ļ�Ѷ��Ѿ�������ȼ�ϣ����������Ӻ��� $1 \operatorname{m}$��

���� $n$ ��ѯ�ʣ�ÿ�θ�һ�������� $q_i$����ʾ��ѯ�� $q_i$ ������ӵ��ƶ����롣

## �����ʽ

**������������������**

��һ��һ�������� $T$����ʾ����������

����ÿ�����ݣ�

��һ����������� $a_1, b_1, a_2, b_2, n$���������Ŀ������

������ $n$ �У�ÿ��һ�������� $q_i$����ʾѯ�ʡ�

## �����ʽ

ÿ��������� $n$ �У���ʾÿ��ѯ�ʵĴ𰸣����� $q_i$ ������ӵ��ƶ����롣

## ���ݷ�Χ

���� $\sum n$ ��ʾ�������ݵ� $n$ ֮�ͣ�$\sum a_1, \sum b_1, \sum a_2, \sum b_2$ ͬ��

$1 \le T \le 10^5$��$1 \le a_1, b_1, a_2, b_2 \le 10^6$��$\sum a_1, \sum b_1, \sum a_2, \sum b_2, \sum n \le 10^6$��$1 \le q_i \le 10^{16}$��

```input1
3
2 3 2 4 2
7
8
1 1 1 1 2
3
4
9 7 10 3 5
5
10
20
30
50
```

```output1
3
4
2
2
5
9
13
18
28
```

