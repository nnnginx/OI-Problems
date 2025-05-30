## 题目描述

我们有一个的矩形房间，被划分成了 $n \times n$ 个大小样的矩形格子。每个格子有两种状态，要么有箱子，要么没有箱子。箱子是一个底面为 $1 \times 1$ 的矩形，高为 $2$、$3$ 或者 $4$ 的长方体。开始时你被困于该房间内的 $S$ 点（必有箱子）上，你想用尽量少的时间要到 $T$ 点，即出口，并且你不能落到地面上。每一时刻，如果你不留在原地发呆，你可以做两件事：

1. 你可以移动到上下左右的某一个相邻的方格内，但是该方格必须有箱子（高度不是问题）；
2. 如果现在你所处的箱子的高度大于 $1$，那么你可以把该箱子向上下左右方向推倒。推倒后原来的位置变空了，推倒后的箱子将覆盖该方向连续的相邻的 height（该箱子的高度）个格子，此时你也将向该方向移动一格。但是要注意，如果你推到箱子后该箱子将倒在其他箱子上或者墙上或者出口上，那么你将不被允许去推倒它。

对于每一件你可以做的事情，它们都耗费 $1$ 的时间。现在你要找出一种方案，使得你可以用最少的时间到达 $T$ 点。

## 输入格式

每个输入文件有多组输入（不超过 $100$ 组），对于每一组数据：

第一行三个数，$n,p,q$，表示房间的长度为 $n(n \le 8)$，你初始的位置为 $(p,q)$，这里使用窗口坐标系。

然后 $n$行，每行 $n$ 个字符，`.` 表示空地，数字 $(2,3,4)$ 表示该位置箱子的高度，`E` 表示该位置为出口。
最后以三个 $0$ 表示输入文件结尾。

## 输出格式

对于每组数据输出一行，表示最短需要的时间。无解则输出 `Impossible`。

## 样例输入

```plain
5 5 3
.2..E
...2.
4....
....4
..2..
0 0 0
```

## 样例输出

```plain
18
```

## 数据规模与约定

$1\le n\le 8$，数据组数不超过 $100$ 组。
