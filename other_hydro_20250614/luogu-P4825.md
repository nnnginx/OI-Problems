## 题目描述
Just like humans enjoy playing the game of Hopscotch, Farmer John's cows have invented a variant of the game for themselves to play. Being played by clumsy animals weighing nearly a ton, Cow Hopscotch almost always ends in disaster, but this has surprisingly not deterred the cows from attempting to play nearly every afternoon.

The game is played on an $R$ by $C$ grid $(2 <= R <= 100,$ $2 <= C <= 100)$, where each square is labeled with an integer in the range $1...K (1 <= K <= R * C)$. Cows start in the top-left square and move to the bottom-right square by a sequence of jumps, where a jump is valid if and only if:

1. You are jumping to a square labeled with a different integer than your current square,

2. The square that you are jumping to is at least one row below the current square that you are on, and

3. The square that you are jumping to is at least one column to the right of the current square that you are on.

Please help the cows compute the number of different possible sequences of valid jumps that will take them from the top-left square to the bottom-right square.

## 输入格式
The first line contains the integers $R, C,$ and $K$. The next $R$ lines will each contain $C$ integers, each in the range $1..K$.

## 输出格式
Output the number of different ways one can jump from the top-left square to the bottom-right square, mod $1000000007$. 

## 题目大意
### 题目描述

与人类喜欢玩跳格子游戏类似，Farmer John 的奶牛们也发明了自己的版本。游戏在一个 $R \times C$ 的网格上进行（$2 \leq R,C \leq 100$），每个格子标有 $1 \ldots K$ 的整数（$1 \leq K \leq R \times C$）。奶牛从左上角出发，通过一系列有效跳跃到达右下角。跳跃被定义为有效当且仅当满足以下条件：

1. 目标格子与当前格子的数字不同  
2. 目标格子位于当前格子下方至少一行  
3. 目标格子位于当前格子右侧至少一列  

请计算从左上角到右下角的不同有效跳跃路径总数。

### 输入格式

第一行包含三个整数 $R$, $C$, $K$。  
接下来 $R$ 行每行包含 $C$ 个整数，每个数在 $1 \ldots K$ 范围内。

### 输出格式

输出从左上角到右下角的不同路径数量，结果对 $1000000007$ 取模。

```input1
4 4 4
1 1 1 1
1 3 2 1
1 2 4 1
1 1 1 1
```

```output1
5
```

