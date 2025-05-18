## 题目描述
Why did the cow cross the road? Well, one reason is that Farmer John's farm simply has a lot of roads, making it impossible for his cows to travel around without crossing many of them.

FJ's farm is arranged as an $N \times N$ square grid of fields ($2 \leq N \leq 100$), Certain pairs of adjacent fields (e.g., north-south or east-west) are separated by roads, and a tall fence runs around the external perimeter of the entire grid, preventing cows from leaving the farm. Cows can move freely from any field to any other adjacent field (north, east, south, or west), although they prefer not to cross roads unless absolutely necessary.

There are $K$ cows ($1 \leq K \leq 100, K \leq N^2$) on FJ's farm, each located in a different field. A pair of cows is said to be "distant" if, in order for one cow to visit the other, it is necessary to cross at least one road. Please help FJ count the number of distant pairs of cows.

## 输入格式
The first line of input contains $N$, $K$, and $R$. The next $R$ lines describe $R$ roads that exist between pairs of adjacent fields. Each line is of the form $r$ $c$ $r'$ $c'$ (integers in the range $1 \ldots N$), indicating a road between the field in (row $r$, column $c$) and the adjacent field in (row $r'$, column $c'$). The final $K$ lines indicate the locations of the $K$ cows, each specified in terms of a row and column.

## 输出格式
Print the number of pairs of cows that are distant.

## 题目大意
### 题目描述

奶牛为什么要过马路？其中一个原因是 Farmer John 的农场有很多道路，使得他的奶牛在四处走动时不可避免地要穿过许多道路。

FJ 的农场被安排成一个 $N \times N$ 的方形网格田地（$2 \leq N \leq 100$），某些相邻的田地（例如南北向或东西向）被道路分隔，整个网格的外部有一圈高高的围栏，防止奶牛离开农场。奶牛可以从任何田地自由移动到相邻的田地（北、东、南或西），尽管它们除非绝对必要，否则不愿意穿过道路。

农场上有 $K$ 头奶牛（$1 \leq K \leq 100, K \leq N^2$），每头奶牛位于不同的田地。如果一头奶牛要拜访另一头奶牛时必须至少穿过一条道路，那么这对奶牛被称为“远距离”对。请帮助 FJ 计算远距离奶牛对的数量。

### 输入格式

输入的第一行包含 $N$、$K$ 和 $R$。接下来的 $R$ 行描述了 $R$ 条存在于相邻田地之间的道路。每行的格式为 $r$ $c$ $r'$ $c'$（范围为 $1 \ldots N$ 的整数），表示位于（行 $r$，列 $c$）的田地与相邻的（行 $r'$，列 $c'$）的田地之间有一条道路。最后的 $K$ 行表示 $K$ 头奶牛的位置，每行用行和列指定。

### 输出格式

输出远距离奶牛对的数量。

```input1
3 3 3
2 2 2 3
3 3 3 2
3 3 2 3
3 3
2 2
2 3
```

```output1
2
```

