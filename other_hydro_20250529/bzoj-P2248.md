

## 题目描述
>John and Brus are playing a military strategic game on a PC. The game is played on the flat world map. At the beginning of the game Brus places his army. Then John has to choose strategic points for his army according to the following rules: 
>each strategic point must be a lattice point (x, y) (a lattice point is a point with integer coordinates) such that |x| + |y| < N; 
John can choose any positive number of strategic points; 
all the strategic points must be distinct; 
each of the strategic points must be free (i.e. not occupied by Brus’s army); 
each pair of different strategic points must be connected (possibly via some other strategic points). 
>Here two different lattice points (x1, y1) and (x2, y2) are connected if |x1 – x2| + |y1 – y2| = 1. If A, B and C are strategic points, A and B are connected, B and C are connected, then A and C are also connected. 
Your task is to find the number of ways for John to choose strategic points for his army.

## 中文翻译

John 和 Brus 正在玩一个军事战略游戏，游戏在一个水平地图上进行，在游戏开始时 Brus 会布置它的军队，然后 John 需要为他的军队选择战略点，选择战略点需遵循如下规则：

- 战略点的坐标 $(x,y)$ 均为整数且满足 $|x|+|y| \lt n$。
- 不同战略点必须互不相同。
- 不能选择 Brus 已经占领的点作为战略点。
- 战略点之间需联通（此处的联通指的是四联通）。

你需要求出 John 放置战略点的方案数。 

## 输入格式
>The first line contains single integer T – the number of test cases. Each test case starts with a line containing two integers N and M separated by a single space. N is the number mentioned in the first rule. M is the number of lattice points on the world map already occupied by Brus’s army. Each of the following M lines contains two integers Xk and Yk separated by a single space. Each lattice point (Xk, Yk) is occupied by Brus’s army.

第一行一个整数 $T$，代表数据组数。

每组数据的第一行包括两个数 $n,m$，其中 $n$ 为第一个限制中的 $n$，$m$ 为 Brus 已经占领的点的个数。

接下来 $m$ 行，每行两个整数 $x,y$，描述了 Brus 占领的点的坐标。
## 输出格式
>For each test case print a single line containing the number of ways for John to choose strategic points for his army.

对每组数据，输出其对应的答案。

```input1
2 
2 1 
7 7 
2 3 
0 0 
4 -7 
7 -4

```
```output1
20 
4

```
$1\le T\le 74,1\le n\le 7,1\le m\le 225,-7\le x,y\le 7$，所有 $x,y$ 互不相同。
## 提示
没有写明提示
## 题目来源
没有写明来源


