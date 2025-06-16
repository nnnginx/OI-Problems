## 题目描述
Bessie has gotten herself stuck on the wrong side of Farmer John's barn again, and since her vision is so poor, she needs your help navigating across the barn.

The barn is described by an $N \times N$ grid of square cells ($2 \leq N \leq 20$), some being empty and some containing impassable haybales. Bessie starts in the lower-left corner (cell 1,1) and wants to move to the upper-right corner (cell $N,N$). You can guide her by telling her a sequence of instructions, each of which is either "forward", "turn left 90 degrees", or "turn right 90 degrees". You want to issue the shortest sequence of instructions that will guide her to her destination. If you instruct Bessie to move off the grid (i.e., into the barn wall) or into a haybale, she will not move and will skip to the next command in your sequence.

Unfortunately, Bessie doesn't know if she starts out facing up (towards cell 1,2) or right (towards cell 2,1). You need to give the shortest sequence of directions that will guide her to the goal regardless of which case is true. Once she reaches the goal she will ignore further commands.



## 输入格式
The first line of input contains $N$.

Each of the $N$ following lines contains a string of exactly $N$ characters, representing the barn. The first character of the last line is cell 1,1. The last character of the first line is cell N, N.

Each character will either be an H to represent a haybale or an E to represent an empty square.

It is guaranteed that cells 1,1 and $N,N$ will be empty, and furthermore it is guaranteed that there is a path of empty squares from cell 1,1 to cell $N, N$.


## 输出格式
On a single line of output, output the length of the shortest sequence of directions that will guide Bessie to the goal, irrespective whether she starts facing up or right.


## 题目大意
### 题目描述

Bessie 又一次被困在了 Farmer John 的谷仓的错误一侧，由于她的视力很差，她需要你的帮助来穿过谷仓。

谷仓由一个 $N \times N$ 的方格网格描述（$2 \leq N \leq 20$），其中一些格子是空的，另一些则包含无法通过的干草堆。Bessie 从左下角（格子 1,1）开始，想要移动到右上角（格子 $N,N$）。你可以通过告诉她一系列指令来引导她，每条指令可以是“前进”、“向左转 90 度”或“向右转 90 度”。你需要给出最短的指令序列，以引导她到达目的地。如果你指示 Bessie 移动到网格外（即撞到谷仓墙壁）或进入干草堆，她将不会移动，并跳过你序列中的下一条指令。

不幸的是，Bessie 不知道她最初是面朝上（朝向格子 1,2）还是面朝右（朝向格子 2,1）。你需要给出一个最短的指令序列，无论她最初面朝哪个方向，都能引导她到达目标。一旦她到达目标，她将忽略后续的指令。

### 输入格式

输入的第一行包含 $N$。

接下来的 $N$ 行每行包含一个长度为 $N$ 的字符串，表示谷仓。最后一行的第一个字符是格子 1,1，第一行的最后一个字符是格子 $N,N$。

每个字符要么是 H 表示干草堆，要么是 E 表示空方格。

保证格子 1,1 和 $N,N$ 是空的，并且保证存在一条从格子 1,1 到格子 $N,N$ 的空方格路径。

### 输出格式

输出一行，表示无论 Bessie 最初面朝哪个方向，都能引导她到达目标的最短指令序列的长度。

```input1
3
EHE
EEE
EEE
```

```output1
9
```

