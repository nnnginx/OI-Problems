## ��Ŀ����

The locations of Farmer John's $n$ cows are described by distinct points in the 2D plane. The cows belong to two different breeds: Holsteins and Guernseys. Farmer John wants to build a rectangular fence with sides parallel to the coordinate axes enclosing only Holsteins, with no Guernseys (a cow counts as enclosed even if it is on the boundary of the fence). Among all such fences, Farmer John wants to build a fence enclosing the maximum number of Holsteins. And among all these fences, Farmer John wants to build a fence of minimum possible area. Please determine this area. A fence of zero width or height is allowable.

**���룺**

����ϵ�ϸ��� $n$ ���㣬�� $H$ �� $G$��һ����������������һ���㡣 ������һ�������� $G$ ���Ұ��������� $H$ ���Ӿ��Σ�Ȼ���ڱ�֤ $H$ ������������Ӿ��ε���С����� ��� $H$ ������������ͱ�֤ $H$ ���ʱ����С���������

## �����ʽ

The first line of input contains $n$. 

Each of the next $n$ lines describes a cow, and contains two integers and a character. The integers indicate a point $(x,y)$ at which the cow is located. The character is $H$ or $G$,indicating the cow's breed. No two cows are located at the same point, and there is always at least one Holstein.

## �����ʽ

Print two integers. The first line should contain the maximum number of Holsteins that can be enclosed by a fence containing no Guernseys,and second line should contain the minimum area enclosed by such a fence.

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

## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ�$1\le n\le 500$��$0\le x,y\le10^3$��

## ��Ŀ��Դ

Gold & ��л18357