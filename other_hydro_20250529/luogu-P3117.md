## ��Ŀ����
The locations of Farmer John's N cows (1 <= N <= 500) are described by distinct points in the 2D plane.  The cows belong to two different breeds: Holsteins and Guernseys.  Farmer John wants to build a rectangular fence with sides parallel to the coordinate axes enclosing only Holsteins, with no Guernseys (a cow counts as enclosed even if it is on the boundary of the fence).  Among all such fences, Farmer John wants to build a fence enclosing the maximum number of Holsteins.  And among all these fences, Farmer John wants to build a fence of minimum possible area.  Please determine this area.  A fence of zero width or height is allowable.


## �����ʽ
The first line of input contains N.  Each of the next N lines describes a cow, and contains two integers and a character. The integers indicate a point (x,y) (0 <= x, y <= 1000) at which the cow is located. The character is H or G, indicating the cow's breed.  No two cows are located at the same point, and there is always at least one Holstein.


## �����ʽ
Print two integers. The first line should contain the maximum number of Holsteins that can be enclosed by a fence containing no Guernseys, and second line should contain the minimum area enclosed by such a fence.

## ��Ŀ����
### ��Ŀ����

ũ��Լ���� $N$ ͷţ��$1 \leq N \leq 500$����λ���ɶ�άƽ���ϻ�����ͬ�ĵ���������Щţ��Ϊ����Ʒ�֣�Holsteins �� Guernseys��ũ��Լ��ϣ������һ������������ƽ�еľ���Χ���������� Holsteins �Ҳ������κ� Guernseys����ʹţλ��Χ���߽���Ҳ��Ϊ��������������������������Χ���У�ũ��Լ��ϣ��ѡ�������� Holsteins ��Χ���������ڶ��������Χ������ѡ�����������С��һ������ȷ��������������Χ���Ŀ�Ȼ�߶�Ϊ�㡣

### �����ʽ

��һ��������� $N$���������� $N$ ��ÿ������һͷţ����������������һ���ַ���������ʾţ���ڵ������ $(x, y)$��$0 \leq x, y \leq 1000$�����ַ�Ϊ H �� G ��ʾţ��Ʒ�֡�û����ͷţλ��ͬһλ�ã������ٴ���һͷ Holstein��

### �����ʽ

���������������һ��Ӧ�����������κ� Guernseys ��Χ���ܰ�Χ����� Holsteins �������ڶ���Ӧ���������������Χ������С�����

```input1
5 
1 1 H 
2 2 H 
3 3 G 
4 4 H 
6 6 H 

```

```output1
2 
1 
```

