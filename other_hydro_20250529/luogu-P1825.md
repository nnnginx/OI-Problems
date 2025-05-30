## 题目描述
This past fall, Farmer John took the cows to visit a corn maze. But this wasn't just any corn maze: it featured several gravity-powered teleporter slides, which cause cows to teleport instantly from one point in the maze to another. The slides work in both directions: a cow can slide from the slide's start to the end instantly, or from the end to the start. If a cow steps on a space that hosts either end of a slide, she must use the slide.

The outside of the corn maze is entirely corn except for a single exit.

The maze can be represented by an N x M (2 <= N <= 300; 2 <= M <= 300) grid. Each grid element contains one of these items:

\* Corn (corn grid elements are impassable) 

\* Grass (easy to pass through!) 

\* A slide endpoint (which will transport a cow to the other endpoint) 

\* The exit

A cow can only move from one space to the next if they are adjacent and neither contains corn. Each grassy space has four potential neighbors to which a cow can travel. It takes 1 unit of time to move from a grassy space to an adjacent space; it takes 0 units of time to move from one slide endpoint to the other.

Corn-filled spaces are denoted with an octothorpe (#). Grassy spaces are denoted with a period (.). Pairs of slide endpoints are denoted with the same uppercase letter (A-Z), and no two different slides have endpoints denoted with the same letter. The exit is denoted with the equals sign (=).

Bessie got lost. She knows where she is on the grid, and marked her current grassy space with the 'at' symbol (@). What is the minimum time she needs to move to the exit space?


## 输入格式
第一行：两个用空格隔开的整数 $N$ 和 $M$。

第 $2\sim N+1$ 行：第 $i+1$ 行描述了迷宫中的第 $i$ 行的情况（共有$M$个字符，每个字符中间没有空格）。

## 输出格式
一个整数，表示起点到出口所需的最短时间。

## 题目大意
奶牛们去一个 $N\times M$ 玉米迷宫，$2 \leq N \leq 300,2 \leq M \leq300$。

迷宫里有一些传送装置，可以将奶牛从一点到另一点进行瞬间转移。这些装置可以双向使用。

如果一头奶牛处在这个装置的起点或者终点，这头奶牛就必须使用这个装置，奶牛在传送过后不会立刻进行第二次传送，即不会卡在传送装置的起点和终点之间来回传送。

玉米迷宫除了唯一的一个出口都被玉米包围。

迷宫中的每个元素都由以下项目中的一项组成：

1. 玉米，`#` 表示，这些格子是不可以通过的。
1. 草地，`.` 表示，可以简单的通过。
1. 传送装置，每一对大写字母 $\tt{A}$ 到 $\tt{Z}$ 表示。
1. 出口，`=` 表示。
1. 起点， `@` 表示

奶牛能在一格草地上可能存在的四个相邻的格子移动，花费 $1$ 个单位时间。从装置的一个结点到另一个结点不花时间。

```input1
5 6
###=##
#.W.##
#.####
#.@W##
######

```

```output1
3
```

## 提示
例如以下矩阵，$N=5,M=6$。

```plain
###=##
#.W.##
#.####
#.@W##
######
```

唯一的一个装置的结点用大写字母 $\tt{W}$ 表示。

最优方案为：先向右走到装置的结点，花费一个单位时间，再到装置的另一个结点上，花费 $0$ 个单位时间，然后再向右走一个，再向上走一个，到达出口处，总共花费了 $3$ 个单位时间。

