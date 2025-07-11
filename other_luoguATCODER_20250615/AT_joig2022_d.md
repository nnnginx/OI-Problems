# AT_joig2022_d いちご 2 (Strawberry 2)

## 题目描述

果物爱好者比太郎决定挑战一次草莓抓取游戏。在他的面前有一个长方形的桌子，这张桌子被分成了 $H$ 行 $W$ 列的网格。在这张桌子上，一共放了 $N$ 个草莓。第 $i$ 个草莓（$1 \leq i \leq N$）放在从上往下数第 $A_i$ 行，从左往右数第 $B_i$ 列的格子中。注意，可能会有多个草莓放在同一个格子里。

比太郎只能从桌子上选择一个 $3 \times 3$ 的方形区域来抓取草莓，这样他就能拿走这个区域内的所有草莓。这一动作只能进行一次。

比太郎想尽可能多地获取草莓。

请根据给定的桌子尺寸和草莓的位置信息，编写程序计算他最多能拿到多少草莓。

## 输入格式

输入从标准输入提供，以以下格式给出：

> $H$ $W$ $N$ $A_1$ $B_1$ $A_2$ $B_2$ $\ldots$ $A_N$ $B_N$

## 输出格式

在标准输出中输出一个整数，表示比太郎最多能拿到的草莓数量。

## 输入输出样例 #1

### 输入 #1

```
4 5
7
1 1
1 5
2 2
2 4
3 3
4 2
4 4
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
3 5
6
1 1
1 2
2 1
2 4
2 4
3 4
```

### 输出 #2

```
4
```

## 输入输出样例 #3

### 输入 #3

```
3 99999
9
1 77813
2 77813
3 77813
1 77814
2 77814
3 77814
1 77815
2 77815
3 77815
```

### 输出 #3

```
9
```

## 输入输出样例 #4

### 输入 #4

```
11 11
20
7 7
6 11
5 7
8 8
9 9
5 5
8 4
4 4
4 8
2 6
1 6
6 2
3 3
9 3
7 5
6 1
10 6
6 10
11 6
3 9
```

### 输出 #4

```
4
```

## 说明/提示

### 约束
- $3 \leq H \leq 1\,000\,000\,000$
- $3 \leq W \leq 1\,000\,000\,000$
- $1 \leq N \leq 60\,000$
- $1 \leq A_i \leq H$ （$1 \leq i \leq N$）
- $1 \leq B_i \leq W$ （$1 \leq i \leq N$）
- 输入的所有值均为整数。

### 子任务
1. (14 分) $H \leq 1,000$，$W \leq 1,000$，$N \leq 20$。
2. (16 分) $H \leq 1,000$，$W \leq 1,000$。
3. (29 分) $H \leq 1,000,000$，$N \leq 500$。
4. (15 分) $H = 3$。
5. (20 分) $H \leq 1,000,000$。
6. (6 分) 无额外限制。

### 评分说明

所有的提交都会在评分系统中自动进行测试。

如果提交的代码对一个子任务的所有测试用例都给出了正确结果，则认为该子任务解答正确。

每次提交的得分是其所通过的所有子任务的分数之和。

该题目最终得分为所有提交中最高的一次得分。

当前得分可以在“提交结果”页面的“我的得分情况”中查看。

### 示例解释

在第一个样例中，草莓的布局如图所示（红色圆圈表示草莓）。通过选择框中区域，比太郎可以拿到 $5$ 个草莓，这是可能的最大数量，所以输出 $5$。此输入样例满足子任务 $1, 2, 3, 5, 6$ 的约束条件。

在第二个样例中，多个草莓可能放在同一个格子里。此样例满足所有子任务的约束条件。

第三个样例满足子任务 $3, 4, 5, 6$ 的约束条件。

第四个样例满足子任务 $1, 2, 3, 5, 6$ 的约束条件。

 **本翻译由 AI 自动生成**