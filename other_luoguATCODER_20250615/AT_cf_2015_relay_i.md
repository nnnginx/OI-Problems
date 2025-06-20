# AT_cf_2015_relay_i Platoon Match

## 题目描述

最近，在某个城市的年轻人中，一种名为「Platoon Match」（小队争霸）的游戏风靡一时。参与者手持水枪，穿上雨衣，在场地内奔跑，以射中敌方队员的次数多少来争夺胜利。

以下是游戏的详细规则：$N$ 个参与者被分为两个队伍（人数不一定均等）。所有人从各自队伍的基地同时出发，在指定的场地内移动，并尽力用水枪击中敌方队员。游戏中被敌方队员击中的人会暂时退出比赛，立刻返回自己的基地，然后重新投入游戏。游戏结束时，每个参与者报告自己被击中的次数和击中敌方的次数，从而决定哪支队伍获胜。

现在，你保存了之前比赛的数据，但没有记录每场比赛的队伍分配情况，只知道每个参与者的击中次数和被击中次数。你需要验证是否有一种合理的分队方式，使得所有参与者的比赛成绩是可能的。

## 输入格式

提供一场 Platoon Match 的记录，格式如下：

> $ N $ $ k1 $ $ d1 $ : $ kN $ $ dN $

其中，$N$ ($2 \leq N \leq 200$) 为参与游戏的人数。$ki$ 和 $di$ ($1 \leq i \leq N$, $0 \leq ki, di \leq 200$) 分别表示第 $i$ 个参与者击中敌方的次数和被敌方击中的次数。

## 输出格式

若存在一种分队方式，使得给定的成绩不矛盾，则输出 `valid`；若无此种分队方式，则输出 `invalid`。注意，输出后应有换行。

### 数据范围与提示

#### 样例解释 1

可以将第 1 个参与者分在队伍 1，第 2 和第 3 个参与者分在队伍 2，这样不会有矛盾。（假设第 1 个参与者分别击中了第 2 个参与者 3 次、第 3 个参与者 4 次，第 2 和第 3 个参与者各击中第 1 个参与者 1 次。）

#### 样例解释 2

无论如何分配队伍都会产生矛盾。

#### 样例解释 3

所有人的击中次数总和与被击中次数总和不一致。

#### 样例解释 4

无论如何分配队伍都不会有矛盾。

 **本翻译由 AI 自动生成**

## 输入输出样例 #1

### 输入 #1

```
3
7 2
1 3
1 4
```

### 输出 #1

```
valid
```

## 输入输出样例 #2

### 输入 #2

```
3
2 5
3 2
4 2
```

### 输出 #2

```
invalid
```

## 输入输出样例 #3

### 输入 #3

```
3
4 1
2 1
1 1
```

### 输出 #3

```
invalid
```

## 输入输出样例 #4

### 输入 #4

```
4
0 0
0 0
0 0
0 0
```

### 输出 #4

```
valid
```