## 题目描述
小 K 终于进了宫殿大门，可是他发现却身陷一个巨大的迷宫之中。当小 K 以坚定的信念通过了一次迷宫后，他发现同样的迷宫又出现了，不过出口发生了变化，这时他才知道这个迷宫需要通过 $m$ 次。

由于小 K 希望尽快逃出这迷宫，所以小 K 又请来了你帮忙。

小 K 在一个迷宫里，迷宫里只有小 K，障碍和出口，都可以用整数坐标 $(x_i,y_i)$ 表示。小 K 可以向上下左右四个平行于某一个坐标轴的方向移动，但是每次移动会向一个方向不断前进直到遇到障碍在障碍的前一个整数点停止，此时小 K 才可以再次进行移动。若所要移动的方向上没有障碍或出口，这次的移动就是非法的。每次往一个方向移动的代价为 $1$，当某次移动过程中经过出口此次游戏胜利。

对于给定的迷宫，有 $n$ 个障碍，小 K 起始坐标 $(X,Y)$，以及 $m$ 个出口（这 $m$ 个出口不同时存在），即小 K 需要通过 $m$ 次迷宫。对于每一个出口，问从同一个起始坐标移动到这个出口的最小代价是多少。
## 输入格式
输入的第 $1$ 行有四个正整数 $n,m,X,Y$，分别描述了障碍的个数，出口的个数，以及起始坐标。

下面 $n$ 行，每行两个正整数 $x_{1i},y_{1i}$，描述了这 $n$ 个障碍的坐标为 $(x_{1i},y_{1i})$。

接下来 $m$ 行，每行两个正整数 $x_{2i},y_{2i}$，描述了这 $m$ 个出口的坐标为 $(x_{2i}, y_{2i})$。

所有整数之间用一个空格隔开，保证所有坐标各不相同。
## 输出格式
输出包括 $1$ 行，总共 $m$ 个数，即对于每一个出口，问从起始点到出口的最小代价为多少，若不能到达则输出 `-1`，数字之间用空格隔开，末尾换行。
## 样例输入
```
7 3 6 4
5 1
4 3
1 4
4 5
3 6
6 7
2 8
1 2
2 2
4 8
```
## 样例输出
```
5 2 3
```

## 数据范围
对于 $100\%$ 的数据，$n \leq 10^5$，$m \leq 10^5$，所有坐标涉及的正整数不大于 $10^8$。

## 题目来源
HNOI2009 集训 Day5。


