# AT_abc368_f [ABC368F] Dividing Game

## 题目描述

给定一个长度为 $ N $ 的正整数列 $ A = (A_1, A_2, \dots, A_N) $，其中每个元素都大于等于 $ 2 $。Anna 和 Bruno 将使用这些整数进行游戏。游戏由 Anna 先手，两人轮流进行以下操作：

- 随意选择一个整数 $ i $（$ 1 \leq i \leq N $）。选择 $ A_i $ 的一个正的除数 $ x $（$ x $ 不能是 $ A_i $ 本身），并将 $ A_i $ 替换为 $ x $。

当某一方无法进行操作时，该方输掉游戏，另一方获胜。双方都采取最优策略时，判断谁会获胜。

## 输入格式

输入从标准输入以以下格式给出：

```
N
A_1 A_2 ... A_N
```

## 输出格式

如果 Anna 获胜，输出 `Anna`；如果 Bruno 获胜，输出 `Bruno`。

## 输入输出样例 #1

### 输入 #1

```
3
2 3 4
```

### 输出 #1

```
Anna
```

## 输入输出样例 #2

### 输入 #2

```
4
2 3 4 6
```

### 输出 #2

```
Bruno
```

## 说明/提示

### 限制

- $ 1 \leq N \leq 10^5 $
- $ 2 \leq A_i \leq 10^5 $
- 所有输入都是整数

### 示例解释 #1

以下是一个可能的游戏过程，但请注意，这并不一定是双方都采取最优策略的情况。例如：

- Anna 将 $ A_3 $ 替换为 $ 2 $。
- Bruno 将 $ A_1 $ 替换为 $ 1 $。
- Anna 将 $ A_2 $ 替换为 $ 1 $。
- Bruno 将 $ A_3 $ 替换为 $ 1 $。
- Anna 无法进行操作，因此 Bruno 获胜。
  实际上，在这个示例中，如果 Anna 采取最优策略，她总是可以获胜。