## ��Ŀ����
There is a travel agency in Adelton town on Zanzibar island. It has decided to offer its clients, besides many other attractions, sightseeing the town. To earn as much as possible from this attraction, the agency has accepted a shrewd decision: it is necessary to find the shortest route which begins and ends at the same place.  Your task is to write a program which finds such a route.

In the town there are $N$ crossing points numbered from $1$ to $N$ and $M$ two-way roads numbered from $1$ to $M$.  Two crossing points can be connected by multipleroads, but no road connects a crossing point with itself.  Each sightseeingroute is a sequence of road numbers $y_1$, ..., $y_k$, $k>2$. The road $y_i(1\le i\le k-1)$ connects crossing points $x_i$ and $x_{i+1}$, the road $y_k$ connectscrossing points $x_k$ and $x_1$. All the numbers $x_1$,...,$x_k$ should be different.The length of the sightseeing route is the sum of the lengths of all roads onthe sightseeing route, i.e. $L(y_1)+L(y_2)+$...$+L(y_k)$ where $L(y_i)$ is thelength of the road $y_i (1\le i\le k)$.  Your program has to find such a sightseeingroute, the length of which is minimal, or to specify that it is not possible, because there is no sightseeing route in the town.


## �����ʽ
The first line of input file TRIP. IN contains two positive integers: the number of crossing points $N \le 100$ and the number of roads $M\le 10000$. Each of the next $M$ lines describes one road. It contains 3 positive integers: the number of its first crossing point, the number of the second one, and the length of the road (a positive integer less than $500$).

## �����ʽ
There is only one line in output file TRIP.OUT. It contains either a string 'No solution.' in case there isn't any sightseeing route, or it contains the numbers of all crossing points on the shortest sightseeing route in the order how to pass them (i.e. the numbers $x_1$ to $x_k$ from our definition of a sightseeing route), separated by single spaces. If there are multiple sightseeing routes of the minimal length, you can output any one of them.

## ��Ŀ����
### ��Ŀ����

��ɣ���Ͷ����İ��¶�������һ�������硣����������������⣬������������Ϊ��ͻ��ṩ����Ĺ۹����Ρ�Ϊ�˴������Ŀ�л�þ����ܶ�����棬������������һ�������ľ�������Ҫ�ҵ�һ��ʼ��ͬһ�ص㲢������ͬһ�ص�����·�ߡ���������Ǳ�дһ���������ҵ�������һ��·�ߡ�

�ڸ����� $N$ �����Ϊ 1 �� $N$ �Ľ���㣬�Լ� $M$ �����Ϊ 1 �� $M$ ��˫���·��������������ͨ��������·���ӣ���û�е�·����ͬһ������㡣ÿ���۹�·�����ɵ�·��� $y_1$, ..., $y_k$ ��ɵ����У����� $k > 2$����· $y_i (1 \le i \le k-1)$ ���ӽ���� $x_i$ �� $x_{i+1}$����· $y_k$ ���ӽ���� $x_k$ �� $x_1$�����еĽ������ $x_1$, ..., $x_k$ Ӧ���ǲ�ͬ�ġ��۹�·�ߵĳ����Ǹ�·�����е�·���ȵ��ܺͣ��� $L(y_1)+L(y_2)+...+L(y_k)$������ $L(y_i)$ �ǵ�· $y_i (1 \le i \le k)$ �ĳ��ȡ���ĳ�����Ҫ�ҵ�����һ���۹�·�ߣ�ʹ�䳤����С������ָ���������ҵ�������·�ߣ���Ϊ������û���κι۹�·�ߡ�

### �����ʽ

�����һ�а������������������������� $N \le 100$ �͵�·������ $M \le 10000$���������� $M$ ��ÿ������һ����·��ÿ�а�����������������һ�������ı�ţ��ڶ��������ı�ţ��Լ���·�ĳ��ȣ�С�� 500 ������������

### �����ʽ

���ֻ��һ�С����û���κι۹�·�ߣ�������ַ��� ��No solution.�������������̹۹�·�������н����ı�ţ���ͨ����˳�����У����Ӷ����е� $x_1$ �� $x_k$�������֮���õ����ո�ָ���**��ĩ��Ӧ�ж���ո���߻��з�**������ж��������ͬ�Ĺ۹�·�ߣ����������������һ����

```input1
5 7
1 4 1
1 3 300
3 1 10
1 2 16
2 3 100
2 5 15
5 3 20
```

```output1
1 3 5 2

```

```input2
4 3
1 2 10
1 3 20
1 4 30
```

```output2
No solution.
```

