## 题目描述
Bessie is hoping to fool Farmer John by building a herd of $K$ realistic robotic cows ($1 \leq K \leq 100,000$).

It turns out that building a robotic cow is somewhat complicated. There are $N$ ($1 \leq n \leq 100,000$) individual locations on the robot into which microcontrollers must be connected (so a single microcontroller must be connected at each location). For each of these locations, Bessie can select from a number of different models of microcontroller, each varying in cost.

For the herd of robotic cows to look convincing to Farmer John, no two robots should behave identically. Therefore, no two robots should have exactly the same set of microcontrollers. For any pair of robots, there should be at least one location at which the two robots use a different microcontroller model. It is guaranteed that there will always be enough different microcontroller models to satisfy this constraint.

Bessie wants to make her robotic herd as cheaply as possible. Help her determine the minimum possible cost to do this!

## 输入格式
The first line of input contains $N$ and $K$ separated by a space.

The following $N$ lines contain a description of the different microcontroller models available for each location. The $i$th such line starts with $M_i$ ($1 \leq M_i \leq 10$), giving the number of models available for location $i$. This is followed by $M_i$ space separated integers $P_{i,j}$ giving the costs of these different models ($1 \le P_{i,j} \le 100,000,000$).

## 输出格式
Output a single line, giving the minimum cost to construct $K$ robots.

## 题目大意
### 题目描述

Bessie 希望通过建造 $K$ 头逼真的机器人奶牛（$1 \leq K \leq 100,000$）来愚弄 Farmer John。

事实证明，建造一头机器人奶牛有些复杂。机器人上有 $N$ 个（$1 \leq N \leq 100,000$）独立的位置需要连接微控制器（因此每个位置必须连接一个微控制器）。对于每个位置，Bessie 可以从多个不同的微控制器模型中选择，每个模型的成本各不相同。

为了让机器人牛群对 Farmer John 看起来逼真，任何两头机器人的行为都不应完全相同。因此，任何两头机器人都不应使用完全相同的微控制器集合。对于任意一对机器人，至少应有一个位置上的微控制器模型不同。保证始终有足够的不同微控制器模型来满足此约束。

Bessie 希望以尽可能低的成本建造她的机器人牛群。请帮助她确定实现这一目标的最小可能成本！

### 输入格式

输入的第一行包含用空格分隔的 $N$ 和 $K$。

接下来的 $N$ 行描述了每个位置可用的不同微控制器模型。第 $i$ 行以 $M_i$（$1 \leq M_i \leq 10$）开头，表示位置 $i$ 可用的模型数量。随后是 $M_i$ 个用空格分隔的整数 $P_{i,j}$，表示这些不同模型的成本（$1 \le P_{i,j} \le 100,000,000$）。

### 输出格式

输出一行，表示建造 $K$ 头机器人的最小成本。

```input1
3 10
4 1 5 3 10
3 2 3 3
5 1 3 4 6 6
```

```output1
61
```

