## 题目描述
The locations of Farmer John's N cows (1 <= N <= 500) are described by distinct points in the 2D plane.  The cows belong to two different breeds: Holsteins and Guernseys.  Farmer John wants to build a rectangular fence with sides parallel to the coordinate axes enclosing only Holsteins, with no Guernseys (a cow counts as enclosed even if it is on the boundary of the fence).  Among all such fences, Farmer John wants to build a fence enclosing the maximum number of Holsteins.  And among all these fences, Farmer John wants to build a fence of minimum possible area.  Please determine this area.  A fence of zero width or height is allowable.


## 输入格式
The first line of input contains N.  Each of the next N lines describes a cow, and contains two integers and a character. The integers indicate a point (x,y) (0 <= x, y <= 1000) at which the cow is located. The character is H or G, indicating the cow's breed.  No two cows are located at the same point, and there is always at least one Holstein.


## 输出格式
Print two integers. The first line should contain the maximum number of Holsteins that can be enclosed by a fence containing no Guernseys, and second line should contain the minimum area enclosed by such a fence.

## 题目大意
### 题目描述

农夫约翰的 $N$ 头牛（$1 \leq N \leq 500$）的位置由二维平面上互不相同的点描述。这些牛分为两个品种：Holsteins 和 Guernseys。农夫约翰希望建造一个边与坐标轴平行的矩形围栏，仅包含 Holsteins 且不包含任何 Guernseys（即使牛位于围栏边界上也视为被包含）。在所有满足条件的围栏中，农夫约翰希望选择包含最多 Holsteins 的围栏。若存在多个这样的围栏，则选择其中面积最小的一个。请确定这个面积。允许围栏的宽度或高度为零。

### 输入格式

第一行输入包含 $N$。接下来的 $N$ 行每行描述一头牛，包含两个整数和一个字符。整数表示牛所在点的坐标 $(x, y)$（$0 \leq x, y \leq 1000$），字符为 H 或 G 表示牛的品种。没有两头牛位于同一位置，且至少存在一头 Holstein。

### 输出格式

输出两个整数。第一行应包含不包含任何 Guernseys 的围栏能包围的最大 Holsteins 数量，第二行应包含满足该条件的围栏的最小面积。

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

