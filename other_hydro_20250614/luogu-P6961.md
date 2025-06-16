## ��Ŀ����


To conduct The World Programming Cup $2112$ a network of wonderful toll roads was build in European part of Russia. This network consists of $m$ bidirectional roads that connect $n$ cities. Each road connects exactly two distinct cities, no two roads connect the same pair of cities, and it is possible to travel from any city to any other city using only this road network. Moreover, to ease the process of charging, no two roads intersect outside of the cities.

Each road is assigned some individual positive cost. Normally, if a driver makes a trip using some of these toll roads, at the end of his journey he would be charged the total cost equal to the sum of individual costs of all roads he has used. To increase the popularity of car travels between two capitals, the operator company Radishchev Inc introduced a special offer: make a journey from Saint Petersburg to Moscow and pay for only $k$ most expensive roads along your path.

Formally, let some path consists of $l$ roads. Denote as $c_{1}$ the cost of the most expensive road along this path, as $c_{2}$ the second most expensive and so on. Thus, we have a sequence $c_{1} \ge c_{2} \ge c_{3} \ge $ . . . $ \ge c_{l}$ of individual costs of all roads along the chosen path. If $l \le k$ , then the path is too short and the driver pays the sum of all individual costs as usual, i.e . $��^{l}_{i=1}c_{i}.$ If $l > k$ , then the driver only pays for $k$ most expensive roads, that is $��^{k}_{i=1}c_{i}.$

As the chief analyst of Radishchev Inc you were assigned a task to compute the cheapest possible journey from Saint Petersburg to Moscow.



## �����ʽ


The first line of the input contains three integers $n , m$ and $k (2 \le n \le 3000 , 1 \le m \le 3000 , 1 \le k < n)$ -- the number of cities, the number of roads in the road network, and the maximum number of roads that one should pay for in a single journey.

Next $m$ lines contain description of roads. Each road description contains three integers $u_{i}, v_{i},$ and $w_{i} (1 \le u_{i}, v_{i} \le n , u_{i} �� v_{i}, 1 \le w_{i} \le 10^{9})$ -- the i-th bidirectional road that connects cities $u_{i}$ and $v_{i}$ with the cost of $w_{i}$ for any direction. It is guaranteed that there is at most one road between each pair of cities and it is possible to get from any city to any other city using only these roads.



## �����ʽ


Print one integer equal to the minimum possible cost of travel from the city number $1$ (Saint Petersburg) to the city number $n (Moscow).$



## ��Ŀ����
�� $n$ ������ $m$ ����·��ÿ����·�����������У�ÿ����·����Ҫ��·�ѡ�

$\mathsf{\color{black}{K}\color{red}{arry5307}}$ ��ӳ��� $1$ ����ǰ������ $n$��������ط��ɷ��棬����һ������ $c$ ���ߵ�·����$\mathsf{\color{black}{K}\color{red}{arry5307}}$ ֻ��Ҫ֧��·����ǰ $k$ ��Ĺ�·�ѣ��� $c<k$ ʱ��Ҫ֧��·����ȫ���Ĺ�·�ѣ���

���� $\mathsf{\color{black}{K}\color{red}{arry5307}}$ ��Ҫ����� $1$ ���� $n$ ����С���ѡ���Ϊ $\mathsf{\color{black}{K}\color{red}{arry5307}}$ æ��д�����⣬����������񽻸����㡣

$2\leq n\leq 3000,1\leq m\leq 3000,1\leq k<n$��

```input1
6 7 2
1 2 6
2 3 1
2 4 3
2 5 5
3 6 10
4 6 9
5 6 8

```

```output1
14

```

```input2
5 5 3
2 1 1
3 2 1
4 3 1
4 5 1
1 5 2

```

```output2
2

```

## ��ʾ
Time limit: 3 s, Memory limit: 512 MB. 



