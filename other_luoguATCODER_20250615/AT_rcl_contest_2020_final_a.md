# AT_rcl_contest_2020_final_a ハイパー覆面すごろく

## 题目描述

新的蛇梯棋由 \\(N + 1\\) 个格子组成，按顺序编号为 \\(0, 1, \ldots, N\\)。\\(0\\) 是起点，\\(N\\) 是终点。
- 掷骰子决定前进的步数。如果超过终点，需要向起点方向折返（具体操作可参阅示例）。
- 恰好到达终点后，玩家需重新从起点出发。
- 每个格子有一个分数 \\(V_i\\)，当玩家停在某个格子上时，格子的分数会计入玩家的总分。
- 游戏开始时，X位于起点，得分为 0。格子分数在第一次停留时才知晓，之后不再改变。

X计划进行 \\(M\\) 次投骰子游戏，并在每次掷骰子前改变骰子某一面的值，使游戏更具挑战性。

该骰子是一个标准的六面骰子，每面起始值分别为 \\(1, 2, 3, 4, 5, 6\\)。在每次投掷前，你可以修改其中一个面的值，范围仍需在 \\(1 \\sim 6\\) 之间，且修改后在后续的掷骰中生效。

请帮助X设计骰子的策略，以便在游戏结束时获得最大的分数。

各个测试用例的得分由以下规则计算：

- 每个测试用例中，X最终获得的分数即为该测试用例的得分。
- 本题共有 50 个测试用例，所有测试用例的得分之和即为该题的总分。

## 输入格式

首先，通过标准输入读取以下内容：

```
N M
```

- \\(N\\) 为拱门格子的数量，\\(N = 500\\)。
- \\(M\\) 为允许的投骰次数，\\(M = 5000\\)。
- **请确保读取所有输入，因为这是评测过程中的必要步骤。**

接下来，通过 \\(M\\) 次交互完成与评测程序的互动，在第 \\(M\\) 次交互后结束程序。

1. 在标准输出中输出六个整数，代表骰子的六个面。

```
d_0 d_1 d_2 d_3 d_4 d_5
```

- 在每次投掷前，骰子的面值最多只能修改一个。
- 游戏开始时的初始值为 \\((1, 2, 3, 4, 5, 6)\\)。

2. 接受来自标准输入的三个整数，表示骰子的结果及影响。

```
d v x
```

- \\(d\\) 表示掷出的骰子面朝上的数字。
- \\(v\\) 是玩家到达该格子后的加分值。
- \\(x\\) 为玩家最终到达并停留的格子编号；如果玩家到达终点，则 \\(x = N\\)。

## 输出格式

无

## 说明/提示

> 关于 \\(V_i\\) 值的生成方式：

- \\(V_N = 5000\\)。
- 其他值通过以下步骤设置，以创建差异化格子区域：

  1. 随机选择一个整数 \\(l\\) 在 \\([1, 10]\\) 内。
  2. 随机选择整数 \\(p\\) 在 \\([1, N-5-l]\\) 内。
  3. 从 \\([1, 200]\\) 内随机选择整数 \\(v\\)。
  4. 对 \\(V_p\) 到 \\(V_{p+l-1}\\) 加 \\(v\\)。

特别提示：\\(V_0, V_{N-5}, V_{N-4}, V_{N-3}, V_{N-2}, V_{N-1} = 0\\)。

### 示例

```
输入：
20 6

输出：
1 2 3 4 5 6
```

在这个例子中，有 20 个除起点外的格子，并允许共掷骰 6 次。输入输出示例在约束 \\(N=500, M=5000\\) 下的运行结果：

```
1 2 3 4 6 6
6 263 6
1 2 3 4 6 6
3 132 9
1 2 3 6 6 6
6 0 15
1 2 6 6 6 6
6 0 19
1 2 6 6 6 3
1 5000 20
1 2 6 3 6 3
6 263 6
```

[测试器下载地址](https://github.com/recruit-communications/rcl-contest-2020/tree/master/final_A/tester/)

 **本翻译由 AI 自动生成**