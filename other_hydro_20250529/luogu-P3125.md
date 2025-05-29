## 题目描述
For Bessie the cow’s birthday, Farmer John has given her free reign over one of his best fields to eat grass.

The field is covered in $N$ patches of grass ($1 \le N \le 1000$), conveniently numbered $1\ldots N$, that each have a distinct quality value.  If Bessie eats grass of quality $Q$, she gains $Q$ units of energy.  Each patch is connected to up to 10 neighboring patches via bi-directional paths, and it takes Bessie $E$ units of energy to move between adjacent patches ($1 \le E \le 1,000,000$).

Bessie can choose to start grazing in any patch she wishes, and she wants to stop grazing once she has accumulated a maximum amount of energy.

Unfortunately, Bessie is a picky bovine, and once she eats grass of a certain quality, she’ll never eat grass at or below that quality level again!  She is still happy to walk through patches without eating their grass; in fact, she might find it beneficial to walk through a patch of high-quality grass without eating it, only to return later for a tasty snack.

Please help determine the maximum amount of energy Bessie can accumulate.

## 输入格式
The first line of input contains $N$ and $E$.  Each of the remaining $N$ lines describe a patch of grass.  They contain two integers $Q$ and $D$ giving the quality of the patch (in the range $1\ldots 1,000,000$) and its number of neighbors.  The remaining $D$ numbers on the line specify the neighbors.

## 输出格式
Please output the maximum amount of energy Bessie can accumulate.

## 题目大意
### 题目描述

为了庆祝奶牛 Bessie 的生日，Farmer John 允许她在他最好的草地上自由吃草。

这片草地被划分为 $N$ 块草皮（$1 \le N \le 1000$），编号为 $1\ldots N$，每块草皮都有一个独特的质量值。如果 Bessie 吃了质量为 $Q$ 的草，她会获得 $Q$ 单位的能量。每块草皮通过双向路径与最多 10 个相邻草皮相连，Bessie 在相邻草皮之间移动需要消耗 $E$ 单位的能量（$1 \le E \le 1,000,000$）。

Bessie 可以选择从任意一块草皮开始吃草，她希望在积累最大能量后停止吃草。

不幸的是，Bessie 是一头挑剔的牛，一旦她吃了某种质量的草，她就再也不会吃质量等于或低于该水平的草了！她仍然乐意在不吃草的情况下穿过草皮；事实上，她可能会发现穿过一块高质量草皮而不吃草是有益的，只是为了稍后再回来享用美味的小吃。

请帮助确定 Bessie 能够积累的最大能量。

### 输入格式

输入的第一行包含 $N$ 和 $E$。接下来的 $N$ 行描述每块草皮。每行包含两个整数 $Q$ 和 $D$，分别表示草皮的质量（范围为 $1\ldots 1,000,000$）和它的邻居数量。该行剩下的 $D$ 个数字指定了邻居的编号。

### 输出格式

请输出 Bessie 能够积累的最大能量。

### 说明/提示

Bessie 从草皮 4 开始，获得 5 单位的能量。然后她沿着路径移动到草皮 5，在移动过程中消耗了 2 单位的能量。她拒绝吃草皮 5 上质量较低的草，并继续移动到草皮 3，再次消耗了 2 单位的能量。最后，她吃了草皮 3 上的草，获得了 6 单位的能量，总共积累了 7 单位的能量。

请注意，上述样例与提交时的测试用例 1 不同。

```input1
5 2
4 1 2
1 3 1 3 4
6 2 2 5
5 2 2 5
2 2 3 4
```

```output1
7
```

## 提示
Bessie starts at patch 4 gaining 5 units of energy from the grass there. She then takes the path to patch 5 losing 2 units of energy during her travel. She refuses to eat the lower quality grass at patch 5 and travels to patch 3 again losing 2 units of energy.  Finally she eats the grass at patch 3 gaining 6 units of energy for a total of 7 energy.

Note that the sample case above is different from test case 1 when you submit.

