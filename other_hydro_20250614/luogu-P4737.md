## ��Ŀ����
A pasture in the wild west can be represented as a rectangular grid embedded in the upper-right quadrant of a standard coordinate system. A herd of $n$ buffalos is scattered throughout the grid, each occupying a unit square. Buffalos are numbered $1$ through $n$; buffalo $j$ is located in the unit square whose upper-right corner is the point with integer coordinates $(x_j,y_j)$. The coordinate axes represent two rivers meeting at the origin, restricting buffalo movement downwards and leftwards.

A total of $m$ settlers arrive, one by one, and each claims a piece of land using the following procedure:
   1.    The settler picks a point with integer coordinates and installs a single fence post at that point.The point he picks is guaranteed to be free of any previously installed fence posts or fences.Moreover, no two fence posts will have the same $x$-coordinate and no two fence posts will have the same $y$-coordinates.
   2.    Starting from the fence post, the settler builds horizontal and vertical fence segments leftwards and downwards, respectively. Each segment is built to be as long as possible �� i. e. until it reaches the river or another fence.
   3.    The settler claims all the land in the connected area bounded with fences and rivers whose upper-right corner is his fence post. Of course, he claims all the buffalos inside as well. Note that settlers arriving later may claim pieces of land already claimed by earlier settlers.

For each settler, find the total number of buffalos he claimed when he arrived.


## �����ʽ
The first line contains an integer $n(1 \le n \le 300 000)$ �� the number of buffalos. The $j-th$ of the following $n$ lines contains two integers $x_j$ and $y_j(1 \le x_j,y_j \le 10^9)$ �� the location of the $j-th$ buffalo.No two buffalos will share the same location.
The following line contains an integer $m(1 \le m \le 300 000)$ �� the number of settlers. The $j-th$ of the following $m$ lines contains two integers $x^{'}_{j}$ and $y^{'}_{j}(1 \le x^{'}_{j},y^{'}_{j} \le 10^9)$ �� the coordinates of the fence postinstalled by the $j-th$ settler. All $x^{'}_{j}$ are different and all $y^{'}_{j}$ are different.


## �����ʽ
Output $m$ lines. The $j-th$ line should contain the number of buffalos claimed by the $j-th$ settler upon arrival.


## ��Ŀ����
**����Ŀ������**

�������˶�ʱ�ڣ�����������һ���������Ա���ʾΪ����ϵ��һ�����е�һ����������� $n$ ͷˮţ�����зֲ��ţ�ÿһͷ��ռ����һ����λ�����Ρ�ˮţ�Ǵ� $1$ �� $n$ ��ţ�$j$ ��ˮţλ�����Ͻ�����Ϊ $(x_j, y_j)$ �ĵ�λ�������С��������ʾ������������ԭ�㴦�ĺ�������ֹˮţ�����·��ƶ���

һ���� $m$ ��ֳ���߽������ÿ���˶�Ҫ����һ�����ص�����Ȩ���������ѭ���¹���

1. ֳ����ѡ��һ����������㣬���ڴ˴���װһ��դ��������ѡ���ĵ����û�б���ǰ��װ��դ����դ����ռ�ݡ����ң�����������դ������ӵ����ͬ�� $x$ ���꣬Ҳ����������դ������ӵ����ͬ�� $y$ ���ꡣ
2. ��դ������ʼ��ֳ���߷ֱ��������²��޽�ˮƽ����ֱ��դ��Ƭ�Ρ�ÿ��դ�����޽��þ����ܳ�����ֱ�������˺�������һ��դ����ͣ�¡�
3. ֳ��������������դ����Ϊ���Ͻǵģ���դ���ͺ�����Χס����ͨ���������Ȩ����Ȼ����Ҳ���������е�����ˮţ������Ȩ��ע�������ֳ����Ҳ�п����������ѱ��ȵ�����ֳ�������ƹ������ء�

����ÿ��ֳ���ߣ�����������յ���ʱ����������������Ȩ��ˮţ��������

**�������ʽ��**

��һ��һ�������� $n$����ʾˮţ�ĸ�����

������ $n$ �У��� $j$ ������������ $x_j, y_j$����ʾ�� $j$ ͷˮţ��λ�ã���������ͷˮţ��λ���غϡ�

������һ��һ�������� $m$����ʾֳ���ߵĸ�����

������ $m$ �У��� $j$ ������������ $x'_j, y'_j$����ʾ�� $j$ ��ֳ���߰�װ��դ������λ�ã����� $x'_j$ ������ͬ������ $y'_j$ ������ͬ��

**�������ʽ��**

��� $m$ �У��� $j$ ��һ����������ʾ�� $j$ ��ֳ���߸յ���ʱ����������������Ȩ��ˮţ��������

**�����ݷ�Χ��**

����ȫ�����ݣ�$1 \le n, m \le 3 \times {10}^5$��$1 \le x_j, y_j, x'_j, y'_j \le {10}^9$�������������� $(x_j, y_j)$ ������ͬ������ $x'_j$ ������ͬ������ $y'_j$ ������ͬ��

**������Դ**��IOI 2021 ��ѵ�ӵ�һ������ҵ��PinkRabbit��

```input1
7
1 1
4 2
6 2
5 3
2 5
4 7
7 5
4
4 4
8 2
9 6
6 5
```

```output1
2
1
3
2
```

