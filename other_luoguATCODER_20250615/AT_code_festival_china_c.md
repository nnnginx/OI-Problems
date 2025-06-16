# AT_code_festival_china_c Regular Polygon

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-festival-2014-china-open/tasks/code_festival_china_c

## 输入格式

Input is given in the following format.

> $ N $ $ x_1 $ $ y_1 $ $ x_2 $ $ y_2 $ : $ x_N $ $ y_N $

- On the first line, you will be given an integer $ N\ (1\ \leq\ N\ \leq\ 1,000) $, the number of integer lattice points given.
- On the following $ N $ lines, you will be given the coordinates of each lattice. The $ i $-th $ (1\ \leq\ i\ \leq\ N) $ line consists of two integers $ x_i,y_i\ (-10^9\ \leq\ x_i,y_i\ \leq\ 10^9) $, the x,y coordinate of the $ i $-th lattice, respectively.
- Each given lattice is guaranteed to be distinct. In other words, for any $ 2 $ integers $ i,j(1\ \leq\ i,j\ \leq\ N) $, if $ i\ \neq\ j $ then $ (x_i,y_i)≠(x_j,y_j) $ holds.

## 输出格式

On the first line, output $ m $, the number of points you chose to make a regular polygon which has most vertices possible.

 On the following $ m $ lines, output the index($ 1 $-indexed) of each points you chose **in ascending order** .

If you cannot make any regular polygon from the given points, just output a single line containing $ 0 $.

## 输入输出样例 #1

### 输入 #1

```
6
1 0
-1 0
0 1
0 -1
1 2
-1 2
```

### 输出 #1

```
4
1
2
3
4
```

## 输入输出样例 #2

### 输入 #2

```
4
0 0
1 0
2 0
3 0
```

### 输出 #2

```
0
```

## 说明/提示

### Problem

You are given $ N $ points of integer lattice on a rectangular coordinate plane, You want to choose some points from them to make a regular polygon by connecting the chosen points with straight lines. Also, you want to choose as many points as possible to make a regular polygon.

Determine the points you should choose to make a regular polygon which has most vertices possible. If there are more than one possible answers, you may choose any one of them.

### Sample Explanation 1

Among the given $ 6 $ points, you can choose $ 4 $ points $ (1,0),(-1,0),(0,1),(0,-1) $ to make a regular square, which has the most vertex possible. So the answer is $ 4 $ and the indices of those points. The $ 4 $ points $ (-1,0),(1,0),(1,2),(-1,2) $ can also make a regular square. So, the indices of them, $ {1,2,5,6} $, will be considered correct too.

### Sample Explanation 2

The given points are on a straight line. You cannot make any regular polygon from them.