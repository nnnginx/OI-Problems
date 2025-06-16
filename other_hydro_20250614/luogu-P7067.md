## ��Ŀ����


Helen is hiking with her friends in a highland. Their plan is to hike from their camp $A$ to a beautiful showplace $B$ .

Unfortunately, Helen started feeling dizzy due to altitude sickness. Help her group find a route such that the topmost height on that route is as small as possible.

![](https://cdn.luogu.com.cn/upload/image_hosting/o2199eky.png)


## �����ʽ


The input file contains full information about the landscape of a square region $10^{6} \times 10^{6}$ in the following format. The first line contains integer $n$ �� the number of triangles in the landscape $(2 \le n \le 2000)$ . Each of following $n$ lines contains nine integers $x_{i_1}, y_{i_1}, z_{i_1}, x_{i_2}, y_{i_2}, z_{i_2}, x_{i3}, y_{i3}, z_{i3}$ �� coordinates of a triangle. All coordinates belong to the closed interval $[0 , 10^{6}]$. The two last lines contain three integers each: $x_{A}, y_{A}, z_{A}$ and $x_{B}, y_{B}, z_{B}$ �� coordinates of the camp A and the showplace $B$ .

The given triangles are guaranteed to describe a consistent continuous landscape. Projections of triangles onto $XY$ plane are non-degenerate and fill the square without overlapping. A vertex of one triangle never lays inside an edge of another triangle. Points $A$ and $B$ belong to the landscape surface and are different.



## �����ʽ


Output a polyline route from $A$ to $B$ with the smallest possible topmost height. The first line should contain $m$ , the number of vertices in this polyline. Each of following $m$ lines should contain three integer coordinates of a polyline vertex: $x_{i}, y_{i},$ and $z_{i}.$ Vertices must be listed along the polyline, from $A$ to $B$ (including these two endpoints).

All coordinates of polyline vertices should be integer. Each polyline edge must belong to some triangle from the input file (possibly, to its edge). The number of vertices in the polyline must not exceed $5n$.



## ��Ŀ����
### ��Ŀ����

H���ں����������ڸ�ԭͽ�������Ǽƻ��Ŵ����ǵ�Ӫ��Aͽ����һ���羰��ʤB��

��ϧ���ǣ�H���˵��ԭ��Ӧ��������������ҵ�һ��·�ߣ�ʹ��·�ߵ���߸߶Ⱦ�����С��
![](https://cdn.luogu.com.cn/upload/image_hosting/o2199eky.png)��$1:10^5$��

### �����ʽ

�������ݰ�������$10^6 \times 10^6$�ĵ�������Ϣ����ʽ���£�

��һ�а�����һ������$n$����ʾ������ռ��ڵ������ε���������������$n$�У�ÿ�а����Ÿ��������ֱ���
$x_{i_1},y_{i_1},z_{i_1},x_{i_2},y_{i_2},z_{i_2},x_{i_3},y_{i_3},z_{i_3}$
����һ�������ε����ꡣÿ�������ε����궼������[$0, 10^6$]֮�䡣������зֱ������A���������B�������ꡣ

�����������α�֤��һ��һ�µ�����ϵ����������XYƽ���ϵ�ͶӰ�ǷǼ򲢵ģ�������������ζ����ص���һ�������εĶ�����Զ����λ����һ�������εı��ڡ�A���B������ͬһ������ϵ�������߲�ͬλ�á�

### �����ʽ

�����A��B��·�ߣ�����߸߶ȿ�����С����һ��Ӧ����m�����˶�����еĶ������������ÿm���߶�Ӧ�ð�������߶���������������ꡣ

���������·���г�����A��B�������������˵㣩��
·�߶�����������궼ӦΪ������ÿ������߱߱������������ļ�����������ߣ��е�ĳ�������Ρ�·�ߵĹյ������ܳ���5n��

```input1
8
1000000 0 0 1000000 1000000 150000 600000 600000 400000
0 1000000 0 600000 600000 400000 600000 1000000 300000
0 1000000 0 400000 300000 150000 600000 600000 400000
400000 0 200000 1000000 0 0 400000 300000 150000
400000 300000 150000 1000000 0 0 600000 600000 400000
600000 600000 400000 1000000 1000000 150000 600000 1000000 300000
0 0 0 400000 0 200000 400000 300000 150000
0 1000000 0 0 0 0 400000 300000 150000
100000 700000 37500
900000 400000 137500

```

```output1
4
100000 700000 37500
400000 300000 150000
900000 150000 100000
900000 400000 137500

```

## ��ʾ
Time limit: 2 s, Memory limit: 256 MB. 



