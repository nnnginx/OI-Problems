## ��Ŀ����
To help capture criminals on the run, the police are introducing a new computer system. The area covered by the police contains N cities and E bidirectional roads connecting them. The cities are labelled 1 to N.

Ϊ�˰���ץ���ӷ�������������һ���µĵ���ϵͳ�������Ͻ������ $N$ �����к� $E$ ��˫���·�����еı���� $1\sim N$��

The police often want to catch criminals trying to get from one city to another. Inspectors, looking at a map, try to determine where to set up barricades and roadblocks. The new computer system should answer the following two types of queries:

���쳣��Ҫץס��Щ������һ�����е��ﷸ�����Ա���ŵ�ͼ������ȷ������������·�ϡ��µļ����ϵͳҪ�ش������������⣺

1. Consider two cities A and B, and a road connecting cities G1 and G2. Can the criminals get
from city A to city B if that one road is blocked and the criminals can't use it?

���ǳ��� $A$ �� $B$���Լ����ӳ��� $G_1$ �� $G_2$ �ĵ�·���ﷸ�ܷ�������·��ͨ������´� $A$ �ӵ� $B$��

2. Consider three cities A, B and C. Can the criminals get from city A to city B if the entire city C is cut off and the criminals can't enter that city?

������������ $A, B, C$���ﷸ�ܷ����޷�ͨ�� $C$ ������´� $A$ �ӵ� $B$?

Write a program that implements the described system.

дһ������ʵ������ϵͳ��

## �����ʽ
The first line contains two integers N and E (2 �� N �� 100 000, 1 �� E �� 500 000), the number of cities and roads.

��һ���������� $N, E$��$2\leq N\leq 10 ^ 5$��$1\leq E\leq 5\times 10 ^ 5$������ʾ���������͵�·������

Each of the following E lines contains two distinct integers between 1 and N �C the labels of two cities connected by a road. There will be at most one road between any pair of cities.

������ $E$ �У�ÿ��������ͬ������ $u, v$����ʾ���Ϊ $u, v$ �ĳ���֮����һ����·��һ�Գ���֮�����ֻ��һ����·��

The following line contains the integer Q (1 �� Q �� 300 000), the number of queries the system is being tested on.

������һ�У�һ������ $Q$��$1\leq Q\leq 3\times 10 ^ 5$������ʾѯ��������

Each of the following Q lines contains either four or five integers. The first of these integers is the type of the query �C 1 or 2.

������ $Q$ �У�ÿ���Ļ������������һ��ѯ�ʡ���һ������ʾѯ�ʵ����� ���� $1$ �� $2$��

If the query is of type 1, then the same line contains four more integers A, B, G1 and G2 as described earlier. A and B will be different. G1 and G2 will represent an existing road.

���ѯ������Ϊ $1$����ô��ͬһ�л����ĸ����� $A, B, G_1, G_2$��$A, B$ ��ͬ���� $G_1, G_2$ ֮����ڵ�·��

If the query is of type 2, then the same line contains three more integers A, B and C. A, B and C will be distinct integers.

���ѯ������Ϊ $2$����ô��ͬһ�л����������� $A, B, C$��$A, B, C$ ������ͬ��

The test data will be such that it is initially possible to get from each city to every other city.

��֤ͼ��ÿ�������໥��ͨ��

## �����ʽ
Output the answers to all Q queries, one per line. The answer to a query can be "yes" or "no".

����ÿ��ѯ�ʣ���� `yes` �� `no` ��ʾ�ش�

```input1
13 15
1 2
2 3
3 5
2 4
4 6
2 6
1 4
1 7
7 8
7 9
7 10
8 11
8 12
9 12
12 13
5
1 5 13 1 2
1 6 2 1 4
1 13 6 7 8
2 13 6 7
2 13 6 8
```

```output1
yes
yes
yes
no
yes
```

## ��ʾ
Croatian Olympiad in Informatics 2007 Task 2

