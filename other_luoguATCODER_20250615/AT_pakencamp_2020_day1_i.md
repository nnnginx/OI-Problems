# AT_pakencamp_2020_day1_i くねくね

## 题目描述

在一个大小为 $H \times W$ 的迷宫中，每个格子可能是墙壁或道路。我们用 `#` 表示墙壁，用 `.` 表示道路。迷宫中的格子坐标以 $(i, j)$ 表示，其中 $i$ 是行号，$j$ 是列号。

现在，鳗鱼位于起始位置 $(sx, sy)$，目标是移动到终点 $(gx, gy)$。每次移动，鳗鱼可以从当前所在的道路格子移动到相邻的道路格子，不能移动到迷宫外或墙壁上。

鳗鱼有个特别的爱好：它喜欢在移动时采用蜿蜒的方式。因此，移动过程中有如下规则：

1. 如果第 $i$ 次移动是上下方向（即垂直移动），那么第 $i+1$ 次移动必须是左右方向（即水平移动）。
2. 如果第 $i$ 次移动是左右方向，则第 $i+1$ 次移动必须是上下方向。
3. 第一次移动不受方向限制，可以选择任何方向。

你的任务是判断鳗鱼能否在遵循上述移动规则的前提下，从起点到达终点。如果能够到达，则输出所需的最少移动次数；如果不能到达，则输出 $-1$。

## 输入格式

输入从标准输入获取，包括：

```
H W
sx sy gx gy
S_{1,1} S_{1,2} ... S_{1,W}
S_{2,1} S_{2,2} ... S_{2,W}
...
S_{H,1} S_{H,2} ... S_{H,W}
```

## 输出格式

如果鳗鱼能够成功迁至目标位置 $(gx, gy)$，输出最少的移动步数；否则，输出 $-1$。请注意在输出的末尾须换行。

## 数据范围与注意事项

- $2 \leq H, W \leq 1000$
- $1 \leq sx, gx \leq H$
- $1 \leq sy, gy \leq W$
- 每个格子状态 $S_{i,j}$ 仅会是 `.`（道路）或 `#`（墙壁）

 **本翻译由 AI 自动生成**

## 输入输出样例 #1

### 输入 #1

```
2 3
1 1 1 3
...
..#
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
3 4
1 1 3 4
....
.#..
....
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
5 7
4 1 5 4
.#..#..
#....#.
...#..#
.#.....
..#..#.
```

### 输出 #3

```
14
```