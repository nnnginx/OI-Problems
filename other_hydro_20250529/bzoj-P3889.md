## ��Ŀ����

Tired of the cold winter weather on her farm, Bessie the cow plans to fly to a warmer destination for vacation. Unfortunately, she discovers that only one airline, Air Bovinia, is willing to sell tickets to cows, and that these tickets are somewhat complicated in structure. 

Air Bovinia owns $n$ planes, each of which flies on a specific "route" consisting of two or more cities. For example, one plane might fly on a route that starts at city 1, then flies to city 5, then flies to city 2, and then finally flies to city 8. No city appears multiple times in a route. If Bessie chooses to utilize a route, she can board at any city along the route and then disembark at any city later along the route. She does not need to board at the first city or disembark at the last city. Each route has a certain cost, which Bessie must pay if she uses any part of the route, irrespective of the number of cities she visits along the route. If Bessie uses a route multiple times during her travel (that is, if she leaves the route and later comes back to use it from antoher city), she must pay for it each time it is used. Bessie would like to find the cheapest way to travel from her farm (in city $s$) to her tropical destination (city $t$). Please help her decide what is the minimum cost she must pay, and also the smallest number of individual flights she must use take to achieve this minimum cost.

**���룺**

Bessie ׼�����ɻ��� $s$ �е� $t$ �С������� $n$ ������ɹ�ѡ��ÿ������ĺ��߶��������������ϵĳ��С���� Bessie ѡ����һ�����ߣ���ô�����ԴӺ���������һ�������Ϸɻ�����;������һ�������·ɻ�������������ĳ�����࣬��ô�ͱ���֧���������Ļ��� $c_i$���������δ��ĳ�����࣬��ô**ÿ�δ�˶�Ҫ֧������**�������ڳ˹���������

�ʣ�Bessie �� $s$ �е� $t$ ������Ҫ������Ǯ���Լ��ڴ˻��������������ηɻ���

## �����ʽ

The first line of input contains $s$, $t$, and $n$, separated by spaces. The next $2\times n$ lines describe the available routes, in two lines per route. The first line contains the cost of using the route $c_i$, and the number of cities along the route $a_i$. The second line contains a list of the cities $d_{i,j}$ in order along the route. Note that the cost of an itinerary can easily add up to more than can fit into a 32-bit integer, so you should probably use 64-bit integers (e.g., "long long" integers in C/C++).

��һ������������ $s,t,n$����ʾ�����㣬�յ�ͺ����������

�������� $2\times n$ �У�ÿ�����С�

��һ��Ϊ����Ļ��� $c_i$������ĺ��߰����ĳ����� $a_i$��

�ڶ���Ϊ�ú������㵽�յ����г��е���� $d_{i,j}$��

���ں��໨�Ѻܹ���Ӧ��ʹ�� $64$ λ��������

## �����ʽ

Output the minimum cost of an itinerary that Bessie can use to travel from city $s$ to city $t$, as well as the minimum number of individual flights required to achieve this minimum cost. 

If there is no solution, output `-1 -1` (quotes for clarity) on a single line.

���һ�С��� Bessie �����ٻ��Ѻ��ڴ˻��������ٳ����ɻ��Ĵ�����������޷��ִ�Ŀ�ĵأ���� `-1 -1`��

```input1
3 4 3
3 5
1 2 3 4 5
2 3
3 5 4
1 2
1 5
```

```output1
2 2
```

## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ�$1\le n \le 10^3$��$1\le c_i \le 10^9$��$1\le a_i \le 100$��$1\le d_{i,j} \le 10^3$��

## ��Ŀ��Դ

Silver