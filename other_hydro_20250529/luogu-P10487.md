## 题目描述
Last night, little erriyue had a horrible nightmare. He dreamed that he and his girl friend were trapped in a big maze separately. More terribly, there are two ghosts in the maze. They will kill the people. Now little erriyue wants to know if he could find his girl friend before the ghosts find them.

You may suppose that little erriyue and his girl friend can move in 4 directions. In each second, little erriyue can move 3 steps and his girl friend can move 1 step. The ghosts are evil, every second they will divide into several parts to occupy the grids within 2 steps to them until they occupy the whole maze. You can suppose that at every second the ghosts divide firstly then the little erriyue and his girl friend start to move, and if little erriyue or his girl friend arrive at a grid with a ghost, they will die.
Note: the new ghosts also can devide as the original ghost.

## 输入格式
The input starts with an integer T, means the number of test cases.

Each test case starts with a line contains two integers n and m, means the size of the maze. (1<n, m<800)

The next n lines describe the maze. Each line contains m characters. The characters may be:
- ‘.’ denotes an empty place, all can walk on.
- ‘X’ denotes a wall, only people can’t walk on.
- ‘M’ denotes little erriyue
- ‘G’ denotes the girl friend.
- ‘Z’ denotes the ghosts.

It is guaranteed that will contain exactly one letter M, one letter G and two letters Z.

## 输出格式
Output a single integer S in one line, denotes erriyue and his girlfriend will meet in the minimum time S if they can meet successfully, or output -1 denotes they failed to meet.

## 题目大意
**【题目描述】**

昨晚，小 erriyue 做了一个可怕的噩梦。他梦到自己和女朋友被困在一个大迷宫里。更可怕的是，迷宫里有两个鬼魂。它们会杀人。现在小 erriyue 想知道在鬼魂找到他们之前，他是否能找到他的女朋友。

假设小 erriyue 和他的女朋友可以向四个方向移动。在每一秒中，小 erriyue 可以移动 $3$ 步，而他的女朋友只能移动 $1$ 步。鬼魂是邪恶的，每一秒它们都会分裂成几部分，占领距离它们两步以内的网格，直到它们占领整个迷宫。你可以假设在每一秒钟，鬼魂首先分裂，然后小 erriyue 和他的女朋友开始移动，如果小 erriyue 或者他的女朋友到达一个有鬼魂的网格，他们就会死亡。

注意：新的鬼魂也可以像原来的鬼魂一样分裂。

**【输入格式】**

输入以一个整数 $T$ 开始，表示测试案例的数量。

每个测试案例以一行开头，包含两个整数 $n$ 和 $m$，表示迷宫的大小。$(1 < n, m < 800)$

接下来的 $n$ 行描述了迷宫。每行包含 $m$ 个字符。字符可能是：
- `.` 表示空地，所有人都可以走。
- `X` 表示墙，只有人类无法行走。
- `M` 表示小 erriyue。
- `G` 表示女朋友。
- `Z` 表示鬼魂。

保证迷宫中恰好有一个字母 `M`、一个字母 `G` 和两个字母 `Z`。

**【输出格式】**

在一行中输出一个整数 $S$，表示如果他们能成功相遇，小 erriyue 和他的女朋友将在最短时间 $S$ 内相遇，或者输出 $-1$ 表示他们未能相遇。

翻译来自于：[ChatGPT](https://chatgpt.com/)

```input1
3
5 6
XXXXXX
XZ..ZX
XXXXXX
M.G...
......
5 6
XXXXXX
XZZ..X
XXXXXX
M.....
..G...

10 10
..........
..X.......
..M.X...X.
X.........
.X..X.X.X.
.........X
..XX....X.
X....G...X
...ZX.X...
...Z..X..X
```

```output1
1
1
-1
```

