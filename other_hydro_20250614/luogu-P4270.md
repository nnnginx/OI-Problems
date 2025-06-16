## 题目描述
Bored of farm life, the cows have sold all their earthly possessions and joined the crew of a traveling circus. So far, the cows had been given easy acts: juggling torches, walking tightropes, riding unicycles -- nothing a handy-hoofed cow couldn't handle. However, the ringmaster wants to create a much more dramatic act for their next show.
The stage layout for the new act involves $N$ platforms arranged in a circle. On each platform, between $1$ and $N$ cows must form a stack, cow upon cow upon cow. When the ringmaster gives the signal, all stacks must simultaneously fall clockwise, so that the bottom cow in a stack doesn't move, the cow above her moves one platform clockwise, the next cow moves two platforms clockwise, and so forth. Being accomplished gymnasts, the cows know they will have no trouble with the technical aspect of this act. The various stacks of cows will not "interfere" with each other as they fall, so every cow will land on the intended platform. All of the cows landing on a platform form a new stack, which does not fall over.

The ringmaster thinks the act will be particularly dramatic if after the stacks fall, the new stack on each platform contains the same number of cows as the original stack on that platform. We call a configuration of stack sizes "magical" if it satisfies this condition. Please help the cows by computing the number of magical configurations. Since this number may be very large, compute its remainder modulo $10^9 + 7$.

Two configurations are considered distinct if there is any platform for which the configurations assign a different number of cows.

## 输入格式
The input is a single integer, $N$ ($1 \leq N \leq 10^{12}$).

## 输出格式
A single integer giving the number of magical configurations modulo $10^9 + 7$.

## 题目大意
### 题目描述

厌倦了农场生活的奶牛们卖掉了所有的财产，加入了一个巡回马戏团。到目前为止，奶牛们被分配了一些简单的表演：杂耍火炬、走钢丝、骑独轮车——没有什么是一头灵巧的奶牛无法应付的。然而，马戏团团长希望为他们的下一场演出创造一个更加戏剧性的表演。

新表演的舞台布局包括 $N$ 个平台，排列成一个圆圈。在每个平台上，必须有 $1$ 到 $N$ 头奶牛堆叠成一摞，奶牛一头叠在另一头上面。当团长发出信号时，所有的堆叠必须同时顺时针倒下，使得堆叠底部的奶牛不动，她上面的奶牛移动一个平台顺时针，再上面的奶牛移动两个平台顺时针，依此类推。作为技艺高超的体操运动员，奶牛们知道她们在技术方面不会有任何问题。各个奶牛堆叠在倒下时不会相互“干扰”，因此每头奶牛都会落在目标平台上。所有落在平台上的奶牛会形成一个新的堆叠，这个堆叠不会倒下。

团长认为，如果堆叠倒下后，每个平台上的新堆叠包含的奶牛数量与原始堆叠相同，那么这个表演将特别戏剧化。我们称满足这一条件的堆叠大小为“魔法”配置。请帮助奶牛们计算魔法配置的数量。由于这个数字可能非常大，请计算其对 $10^9 + 7$ 取模的结果。

如果两个配置在任何平台上分配的奶牛数量不同，则认为它们是不同的配置。

### 输入格式

输入是一个整数 $N$（$1 \leq N \leq 10^{12}$）。

### 输出格式

输出一个整数，表示魔法配置的数量对 $10^9 + 7$ 取模的结果。

### 提示

对于 $N = 4$，有效的配置是 $(1,1,1,1)$、$(2,2,2,2)$、$(3,3,3,3)$、$(4,4,4,4)$、$(2,3,2,3)$ 和 $(3,2,3,2)$。

题目来源：Dhruv Rohatgi

```input1
4
```

```output1
6
```

## 提示
For $N = 4$, the valid configurations are $(1,1,1,1)$, $(2,2,2,2)$, $(3,3,3,3)$, $(4,4,4,4)$, $(2,3,2,3)$, and $(3,2,3,2)$.

Problem credits: Dhruv Rohatgi

