## ��Ŀ����
Ferries crossing the Strait of Gibraltar from Morocco to Spain must carefully navigate to avoid the heavy ship traffic along the strait. Write a program to help ferry captains find the largest gaps in strait traffic for a safe crossing.

Your program will use a simple model as follows. The strait has several parallel shipping lanes in east-west direction. Ships run with the same constant speed either eastbound or westbound. All ships in the same lane run in the same direction. Satellite data provides the positions of the ships in each lane. The ships may have different lengths. Ships do not change lanes and do not change speed for the crossing ferry.

The ferry waits for an appropriate time when there is an adequate gap in the ship traffic. It then crosses the strait heading northbound along a north-south line at a constant speed. From the moment a ferry enters a lane until the moment it leaves the lane, no ship in that lane may touch the crossing line. Ferries are so small you can neglect their size. Figure 1 illustrates the lanes and ships for Sample Input 1. Your task is to find the largest time interval within which the ferry can safely cross the strait.

  ![](https://vj.z180.cn/186da23b465c6f0f9a3f8b946eb2e17d?v=1601909422) 

   Figure 1: Sample Input 1. 

## �����ʽ
The first line of input contains six integers: the number of lanes $n$ ($1 \leq n \leq 10^5$), the width $w$ of each lane ($1 \leq w \leq 1\, 000$), the speed $u$ of ships and the speed $v$ of the ferry ($1 \leq u, v \leq 100$), the ferry��s earliest start time $t_1$ and the ferry��s latest start time $t_2$ ($0 \leq t_1 < t_2 \leq 10^6$). All lengths are given in meters, all speeds are given in meters/second, and all times are given in seconds.

Each of the next $n$ lines contains the data for one lane. Each line starts with either E or W, where E indicates that ships in this lane are eastbound and W indicates that ships in this lane are westbound. Next in the line is an integer $m_ i$, the number of ships in this lane ($0 \leq m_ i \leq 10^5$ for each $1 \leq i \leq n$). It is followed by $m_ i$ pairs of integers $l_{ij}$ and $p_{ij}$ ($1 \leq l_{ij} \leq 1\, 000$ and $-10^6 \leq p_{ij} \leq 10^6$). The length of ship $j$ in lane $i$ is $l_{ij}$, and $p_{ij}$ is the position at time $0$ of its forward end, that is, its front in the direction it moves.

Ship positions within each lane are relative to the ferry��s crossing line. Negative positions are west of the crossing line and positive positions are east of it. Ships do not overlap or touch, and are sorted in increasing order of their positions. Lanes are ordered by increasing distance from the ferry��s starting point, which is just south of the first lane. There is no space between lanes. The total number of ships is at least $1$ and at most $10^5$.

## �����ʽ
Display the maximal value $d$ for which there is a time $s$ such that the ferry can start a crossing at any time $t$ with $s \leq t \leq s+d$. Additionally the crossing must not start before time $t_1$ and must start no later than time $t_2$. The output must have an absolute or relative error of at most $10^{-3}$. You may assume that there is a time interval with $d > 0.1$ seconds for the ferry to cross.

## ��Ŀ����
��Ħ��紩Խֱ�����Ӻ�Ͽ���������Ķ��ֱ���С�ĵغ��У��Ա��⺣Ͽ�ذ��ķ�æ��ֻ��ͨ����дһ�����򣬰������ִ����ҵ���Ͽ��ͨ�����Ҵ����Ĳ�࣬�Ա㰲ȫ��Խ��

���ĳ���ʹ��һ���򵥵�ģ�ͣ�������ʾ����Ͽ�м������������ƽ�к�������������ͬ�ĺ㶨�ٶ��򶫻�������ʻ��ͬһ�����ϵ����д�ֻ����ͬһ������ʻ�����������ṩ��ÿ��ˮ���ϴ�ֻ��λ�á���Щ�������в�ͬ�ĳ��ȡ���������ı亽����Ҳ����ı�������ֵ��ٶȡ�

��������ͨ���㹻�ļ�϶ʱ�����ֻ�ȴ��ʵ���ʱ�䡣Ȼ�����Ժ㶨���ٶ������ϱ�������ʻ������Ͽ���Ӷ��ֽ���ˮ������һ����ֱ�����뿪ˮ������һ�̣���ˮ���ϵĴ�ֻ�����ô��������ߡ����ֺ�С����������Ժ������ǵĳ��ȡ������������ҵ����ֿ��԰�ȫ��Խ��Ͽ�����ʱ������


����ĵ�һ�а�������������ˮ����$n$($1��n��10^5$)��ÿ��ˮ���Ŀ��$w$($1��w��1000$)������$u$�Ͷɴ��ٶ�$v$ ($1��u,v��100$)�����ֵ����翪ʼʱ��$t1$�Ͷ��ֵ�����ʼʱ��$t2$($0��t1<t2��10^6$)�����г��Ⱦ�����Ϊ��λ�������ٶȾ�����/��Ϊ��λ������ʱ�������Ϊ��λ��

��������$n$���е�ÿһ�ж�����һ��ˮ�������ݡ�ÿ���� E �� W ��ͷ������ E ��ʾ�˳����еĴ�������ʻ��W ��ʾ��ˮ���еĴ���������ʻ�����е���һ��������$m_i$����ʾ���������ϵĴ�ֻ����($0��m_i��10^5$ for each $1��i��n$)�� ����������$m_i$��$l_{ij}$�� $p_{ij}$($1��l_{ij}��1000$ and $-10^6��p_{ij}��10^6$)��$l_{ij}$��ʾ��$j$�ڳ���$i$�ϵĳ��ȣ�$p_{ij}$����ǰ����ʱ��$0$��λ�ã�����ǰ�������ƶ������ϵ�λ�á�

ÿ�������ڵĴ���λ������ڶ��ֵĽ����ߡ�����λλ�ڽ���������������λλ�ڽ������Զ�����ֻ���ص���Ӵ���������λ�õĵ���˳�����򡣳�����˳����������������ľ��룬�����λ�ڵ�һ���������ϱߡ�����֮��û�пռ䡣������������Ϊ
$1$�����$10^5$��


���������ʱ��$s$�����ֵ$d$���Ա�ɴ��������κ�ʱ��t��ʼ��Խ��Ͽ��$s��t��s+d$.
���⣬��ɲ�����ʱ��$t1$֮ǰ��ʼ�����Ҳ�������ʱ��$t2$��ʼ������ľ��Ի�������������Ϊ$10^{-3}$�������Լ������ͨ����ʱ����Ϊ$d$��$d>0.1$�� �롣


ʱ�����ƣ�3000ms���ڴ����ƣ�1048576KB��

```input1
3 100 5 10 0 100
E 2 100 -300 50 -100
W 3 10 60 50 200 200 400
E 1 100 -300

```

```output1
6.00000000

```

```input2
1 100 5 10 0 200
W 4 100 100 100 300 100 700 100 900

```

```output2
50.00000000

```

## ��ʾ
Time limit: 3000 ms, Memory limit: 1048576 kB. 

 International Collegiate Programming Contest (ACM-ICPC) World Finals 2015

