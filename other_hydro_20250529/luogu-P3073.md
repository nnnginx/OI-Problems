## 题目描述
One of Farmer John's fields is particularly hilly, and he wants to purchase a new tractor to drive around on it.  The field is described by an N x N grid of non-negative integer elevations (1 <= N <= 500).  A tractor capable of moving from one grid cell to an adjacent cell (one step north, east, south, or west) of height difference D costs exactly D units of money.

FJ would like to pay enough for his tractor so that, starting from some grid cell in his field, he can successfully drive the tractor around to visit at least half the grid cells in the field (if the number of total cells in the field is odd, he wants to visit at least half the cells rounded up).  Please help him compute the minimum cost necessary for buying a tractor capable of this task.


## 输入格式
\* Line 1: The value of N.

\* Lines 2..1+N: Each line contains N space-separated non-negative integers (each at most 1 million) specifying a row of FJ's field.






## 输出格式
\* Line 1: The minimum cost of a tractor that is capable of driving around at least half of FJ's field.




## 题目大意
题目描述

FJ有块农田太崎岖了，他要买一辆新拖拉机才能在这里巡视。这块农田由N x N个格子的非负整数表示高度(1<=N<=500)。拖拉机从当前格子走到相邻格子（东、南、西、北四个方向）的代价为高度差D，则FJ驶过这两个格子的拖拉机最少也要值D块钱。

FJ愿意花足够的钱买一辆新的拖拉机使得他能以最小的高度差走遍所有格子的一半(如果格子总数是奇数，那么一半的值为四舍五入的值)。因为FJ很懒，所以他找到你帮他编程计算他最小需要花多少钱买到符合这些要求的拖拉机。

输入输出格式

输入格式：

第一行为一个整数N

第2到N+1行每行包含N个非负整数（不超过1,000,000），表示当前格子的高度。

输出格式：

共一行，表示FJ买拖拉机要花的最小价钱。

```input1
5 
0 0 0 3 3 
0 0 0 0 3 
0 9 9 3 3 
9 9 9 3 3 
9 9 9 9 3 

```

```output1
3 

```

