## ��Ŀ����
Tired of the cold winter weather on her farm, Bessie the cow plans to fly to a warmer destination for vacation. Unfortunately, she discovers that only one airline, Air Bovinia, is willing to sell tickets to cows, and that these tickets are somewhat complicated in structure.

Air Bovinia owns N planes (1 <= N <= 1000), each of which flies on a specific "route" consisting of two or more cities.  For example, one plane might fly on a route that starts at city 1, then flies to city 5, then flies to city 2, and then finally flies to city 8. No city appears multiple times in a route. If Bessie chooses to utilize a route, she can board at any city along the route and then disembark at any city later along the route. She does not need to board at the first city or disembark at the last city. Each route has a certain cost, which Bessie must pay if she uses any part of the route, irrespective of the number of cities she visits along the route. If Bessie uses a route multiple times during her travel (that is, if she leaves the route and later comes back to use it from antoher city), she must pay for it each time it is used.

Bessie would like to find the cheapest way to travel from her farm (in city A) to her tropical destination (city B). Please help her decide what is the minimum cost she must pay, and also the smallest number of individual flights she must use take to achieve this minimum cost.


## �����ʽ
The first line of input contains A, B, and N, separated by spaces.

The next 2N lines describe the available routes, in two lines per route. The first line contains the cost of using the route (an integer in the range 1..1,000,000,000), and the number of cities along the route (an integer in the range 1..100).  The second line contains a list of the cities in order along the route.  Each city is identified by an integer in the range 1..1000. Note that the cost of an itinerary can easily add up to more than can fit into a 32-bit integer, so you should probably use 64-bit integers (e.g., "long long" integers in C/C++).


## �����ʽ
Output the minimum cost of an itinerary that Bessie can use to travel from city A to city B, as well as the minimum number of individual flights required to achieve this minimum cost. If there is no solution, output "-1 -1" (quotes for clarity) on a single line.


## ��Ŀ����
### ��Ŀ����

Bessie ����ũ���Ǻ���������е��ᷳ��������׼�����ɻ���һ������ů�ĵط��ȼ١����ҵ��ǣ�������ֻ��һ�����չ�˾��Air Bovinia��Ը����Ʊ��ţ��������ЩƱ�Ľṹ��Щ���ӡ�

Air Bovinia ӵ�� $n$ �ܷɻ���ÿ�ܷɻ�����һ���������������ϵĳ��е����⺽�ߡ��ٸ����ӣ�һ�ܷɻ����Դӳ��� $1$ ������Ȼ��������� $5$���ٷɵ����� $2$�����ɵ����� $8$��ע��**�����ǵ����**���κγ��ж�������ͬһ�������ϳ��ֶ�Ρ���� Bessie ѡ����һ�����ߣ���ô�����ԴӺ����ϵ�����һ�������Ϸɻ���Ȼ����;������һ�������·ɻ��������شӺ��ߵ�����Ϸɻ����ٴӺ��ߵ��յ��·ɻ���ÿ�����߶���һ��ȷ���Ļ��ѣ�ֻҪ�������������࣬���ͱ���֧����������ȫ��ѣ�������;���˼������С���� Bessie ��δ����ĳ�����࣬��ôÿ�δ�� Bessie ������֧������Ļ��ѡ�

Bessie ��Ҫ�ҵ�����ũ�����ڵĳ��У����� $A$������Ŀ�ĵ����ڳ��У����� $B$������˵�·�ߡ����������������Ҫ������Ǯ�����������ڴ˻�����������Ҫ**�������κ���**��Ҳ�������ĳ������� $-1$�����������յ㣩��

### �����ʽ

��һ���������� $A,B,n$��

������ $2n$ �У�ÿ��������һ�κ��ࡣ��һ�а������ߵĻ��� $cost$ �뾭���ĳ����� $len$���ڶ��� $len$ ����������ʾ�������ξ����ĳ��С�

### �����ʽ

һ��������������� Bessie ��������Ҫ����Ǯ�Լ��ڴ˻��������ٵľ�������������

��� Bessie ���ܴ�����ũ����������Ŀ�ĵأ������ `-1 -1`��

### ���ݷ�Χ

$1\le n\le 1000$��$1\le cost\le 10^9$��$1\le len\le 100$�����еı�ž������� $1000$��

������Ҫ�� `long long`��


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

