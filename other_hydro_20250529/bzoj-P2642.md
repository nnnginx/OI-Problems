## 题目描述

我方现在有 $N$ 个据点，司令部建立这些点围成的区域中。现在敌人准备爆掉其中一些点。使得无论我方将司令部建在哪里，最终都不会在剩下的点围成的区域中。

![pic1](./2192/file/pic1.JPG)

## 输入格式

The first line of the input file contains a single integer $n$ — the number of watchtowers. The next $n$ lines of the input file contain the Cartesian coordinates of watchtowers, one pair of coordinates per line. Coordinates are integer and do not exceed $10^{6}$ by absolute value. Towers are listed in the order of traversal of their convex hull in clockwise direction.

## 输出格式

Write to the output file the number of watchtowers the enemy has to blow up to compromise headquarters protection if the headquarters are placed optimally.

## 样例

```input1
5
0 0
0 10
10 20
20 10
25 0

```

```output1
2
```


## 数据规模与约定

对于 $100\%$ 的数据， $3 \leq n \leq 5 \times 10^4$。

## 来源

Pku3968
