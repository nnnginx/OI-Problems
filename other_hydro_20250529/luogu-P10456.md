## 题目描述
The game “The Pilots Brothers: following the stripy elephant” has a quest where a player needs to open a refrigerator.

There are $16$ handles on the refrigerator door. Every handle can be in one of two states: open or closed. The refrigerator is open only when all handles are open. The handles are represented as a matrix $4\times4$. You can change the state of a handle in any location $[i, j] (1 \leq i, j \leq 4)$. However, this also changes states of all handles in row $i$ and all handles in column $j$.

The task is to determine the minimum number of handle switching necessary to open the refrigerator.

## 输入格式
The input contains four lines. Each of the four lines contains four characters describing the initial state of appropriate handles. A symbol “+” means that the handle is in closed state, whereas the symbol “−” means “open”. At least one of the handles is initially closed.

## 输出格式
The first line of the input contains $N$ – the minimum number of switching. The rest $N$ lines describe switching sequence. Each of the lines contains a row number and a column number of the matrix separated by one or more spaces. If there are several solutions, you may give any one of them.

## 题目大意
**【题目描述】**

游戏《飞行员兄弟：追寻条纹大象》中有一个任务，玩家需要打开一个冰箱。

冰箱门上有 $16$ 个手柄。每个手柄可以处于两种状态之一：打开或关闭。只有当所有手柄都打开时，冰箱才会打开。手柄被表示为一个 $4\times4$ 的矩阵。你可以改变任何位置 $[i, j] (1 \leq i, j \leq 4)$ 处手柄的状态。但是，这也会改变第 $i$ 行和第 $j$ 列中所有手柄的状态。

任务是确定打开冰箱所需的最小切换次数。

**【输入格式】**

输入包含四行。每一行都包含四个字符，描述相应手柄的初始状态。符号 “+” 表示手柄处于关闭状态，而符号 “−” 表示 “打开”状态。至少有一个手柄最初是关闭的。

**【输出格式】**

输入的第一行包含 $N$ - 最小切换次数。接下来的 $N$ 行描述切换序列。每行包含一个矩阵的行号和列号，用一个或多个空格分隔开。如果存在多个解决方案，则可以提供任何一个解决方案。

翻译来自于：ChatGPT。

```input1
-+--
----
----
-+--
```

```output1
6 
1 1 
1 3 
1 4 
4 1 
4 3 
4 4
```

