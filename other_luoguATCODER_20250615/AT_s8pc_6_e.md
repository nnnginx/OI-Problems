# AT_s8pc_6_e 90-degree Rotations

## 题目描述

在一个 $H \times W$ 的网格棋盘上，有些格子放置了硬币。用坐标 $(i, j)$ 表示棋盘上第 $i$ 行第 $j$ 列的格子。

若 $S_{i, j} = \texttt{o}$，说明格子 $(i, j)$ 上有一枚硬币；如果 $S_{i, j} = \texttt{x}$，则格子上没有硬币。

E869120 君可以选择一枚硬币所在的格子作为机器人的起始位置，并选择一个方向（上下左右之一）作为机器人的初始朝向。

机器人可以反复执行以下操作：

- 取走当前格子上的硬币，然后选择向左或向右旋转 $90$ 度，接着跳到下一个有硬币的格子。

请问，通过合理选择起始位置、方向、跳跃和旋转，E869120 君能否收集所有硬币？

## 输入格式

输入提供如下格式：

> $H$ $W$ $S_{1, 1}S_{1, 2}S_{1, 3}\ldots S_{1, W}$ $S_{2, 1}S_{2, 2}S_{2, 3}\ldots S_{2, W}$ \[...\] $S_{H, 1}S_{H, 2}S_{H, 3}\ldots S_{H, W}$

## 输出格式

如果有方法可以收集到所有硬币，输出 `Possible`；否则，输出 `Impossible`。

## 输入输出样例 #1

### 输入 #1

```
5 5
xooxx
xoxxo
xxoox
ooxoo
xoxxx
```

### 输出 #1

```
Possible
```

## 输入输出样例 #2

### 输入 #2

```
2 9
oxxxxoxxo
oxoxxoxxo
```

### 输出 #2

```
Possible
```

## 输入输出样例 #3

### 输入 #3

```
9 25
xxxxxxxxxxxxxxxxxxxxxxxxx
xxoooxxxoooxxooooxxxoooxx
xoxxxoxoxxxoxoxxxoxoxxxox
xoxxxxxoxxxoxoxxxoxoxxxxx
xxoooxxxoooxxooooxxoxxxxx
xxxxxoxoxxxoxoxxxxxoxxxxx
xoxxxoxoxxxoxoxxxxxoxxxox
xxoooxxxoooxxoxxxxxxoooxx
xxxxxxxxxxxxxxxxxxxxxxxxx
```

### 输出 #3

```
Impossible
```

## 输入输出样例 #4

### 输入 #4

```
6 6
oxxxxo
xoooxx
xoooox
xoooox
xxooxx
oxxxxo
```

### 输出 #4

```
Impossible
```

## 说明/提示

### 限制条件

- $2 \leq H \leq 100$
- $2 \leq W \leq 100$
- 每个 $S_{i, j}$ 为 `o` 或 `x`
- 棋盘上至少有一枚硬币

### 部分分数

题目分为若干小任务。如果代码通过了某个小任务的所有测试用例，则认为该任务成功。代码的总得分为成功通过所有小任务的得分之和。

1. (100 分)：棋盘上硬币数 $N \leq 8$
2. (110 分)：$N \leq 16$
3. (150 分)：棋盘高度 $H = 2$
4. (440 分)：无其他限制

### 示例解释

在示例 1 中，可以通过一定顺序和方式移动机器人，成功收集所有硬币。  
在示例 2 中，也可以通过合理移动机器人，达到收集不断硬币的目的。  
在示例 3 与示例 4 中，任何尝试都无法收集所有硬币。

 **本翻译由 AI 自动生成**