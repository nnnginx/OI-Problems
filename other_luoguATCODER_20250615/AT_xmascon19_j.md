# AT_xmascon19_j Sub-Post Correspondence Problem

## 题目描述

有 $N$ 种各 $2019^{2019}$ 张的卡片。

第 $i$ 种卡片的上侧印有字符串 $A_i$，下侧印有字符串 $B_i$。

现在，从这些卡片中选择至少一张卡并按任意顺序排列成一列。排列后，上侧字符串连接成一个整体形成字符串 $s$，下侧字符串连接成另一个整体形成字符串 $t$。

请问，是否可以通过选择和排列卡片，使得可以通过删除 $s$ 的任意字符来使其变成 $t$？

## 输入格式

第一行输入一个整数 $N$。
接下来的 $N$ 行中，每行包含两个字符串 $A_i$ 和 $B_i$。

## 输出格式

如果可以满足条件地选择并排列卡片，输出 `YES`；否则，输出 `NO`。

## 输入输出样例 #1

### 输入 #1

```
2
cab ac
acba ab
```

### 输出 #1

```
YES
```

## 输入输出样例 #2

### 输入 #2

```
1
xmas contest
```

### 输出 #2

```
NO
```

## 说明/提示

- $1 \leq N \leq 16$。
- $1 \leq |A_i|, |B_i| \leq 10^5$。
- $A_i$ 和 $B_i$ 仅由小写字母组成。

### 样例解释

例如，按第 2 种、再第 2 种、最后第 1 种的顺序排列卡片，得到 $s = $`acbaacbacab` 和 $t = $`ababac`，满足题目条件。

 **本翻译由 AI 自动生成**