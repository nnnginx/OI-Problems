# AT_wupc2019_d Choose Your Characters

## 题目描述

卡托君和他的好朋友信也君很喜欢一起玩一款去年年底发布的热门动作游戏。

在这个游戏中，有 \\(N\\) 种角色，每个角色都被分配了编号 \\(1, 2, \cdots, N\\)。两位玩家分别从中选择一个角色进行对战。角色之间存在三种相性关系：“有利”、“不利”和“平分”。

- 如果角色 \\(i\\) 对角色 \\(j\\) 有利：
  - 那么当对手选择角色 \\(j\\) 而你选择角色 \\(i\\) 时，你的优势更明显。
- 如果角色 \\(i\\) 对角色 \\(j\\) 不利：
  - 那么当对手选择角色 \\(j\\) 而你选择角色 \\(i\\) 时，你会受到不利影响。
- 如果角色 \\(i\\) 和角色 \\(j\\) 平分：
  - 则两者对战时不受相性影响。

此外，角色 \\(i\\) 若对角色 \\(j\\) 有利，则角色 \\(j\\) 必定对角色 \\(i\\) 不利。

由于卡托君不愿输给信也君，他决定只专注练习部分角色。

具体而言，他会从所有角色中选一个区间 \\([L, R]\\) 来练习这些角色。

为了增加比赛的胜算，卡托君希望选择的区间满足以下条件：

- 无论对手选择哪个角色，区间内至少存在一个角色对该对手角色具有平分或优势。注意，不能选择对手选的那个相同角色。

卡托君平时学习很忙，希望练习的角色数量越少越好。请帮他找出需要练习的角色。

## 输入格式

输入由以下格式提供：

```
\(N\)
\(M\)
\(a_1\) \(b_1\)
\(a_2\) \(b_2\)
\(\vdots\)
\(a_M\) \(b_M\)
```

## 输出格式

输出满足条件的最小区间 \\(L, R\\) \\((L \leq R)\\)，用空格隔开。如果有多个长度相同的最小区间，则选择 \\(L\\) 值最小的那个。

如果没有符合条件的区间，输出 `-1`。

```
\(L\) \(R\)
```

## 输入输出样例 #1

### 输入 #1

```
3
2
2 1
3 1
```

### 输出 #1

```
2 3
```

## 输入输出样例 #2

### 输入 #2

```
3
2
1 2
3 2
```

### 输出 #2

```
1 3
```

## 输入输出样例 #3

### 输入 #3

```
3
2
2 1
2 3
```

### 输出 #3

```
-1
```

## 输入输出样例 #4

### 输入 #4

```
5
8
1 2
2 3
3 1
1 5
5 4
4 1
4 2
5 3
```

### 输出 #4

```
1 3
```

## 说明/提示

- \\(2 \leq N \leq 10^5\\)
- \\(1 \leq M \leq \min(2 \times 10^5, N(N-1)/2)\\) 
  - 表示记录有利、不利关系的数量。
- \\(1 \leq a_i, b_i \leq N\\)，且 \\(a_i \neq b_i\\)
  - 表示角色 \\(a_i\\) 对角色 \\(b_i\\) 有利。
- 保证不会出现与题意相悖的输入：
  - 对于 \\(i \neq j\\)，不同的关系不会重复出现；正反关系不会共同出现。
- 输入值均为整数。
- 未在输入中涉及的相性默认为平分。

### 示例解释 1

比如，对于角色 \\(1\\) 和角色 \\(3\\)，选择角色 \\(2\\)；对于角色 \\(2\\)，选择角色 \\(3\\)。这样可以保证无论对手选择哪个角色，都能有至少平分的相性。

### 示例解释 2

例如，对于角色 \\(1\\) 和角色 \\(2\\)，选择角色 \\(3\\)；对于角色 \\(3\\)，选择角色 \\(1\\)。这样无论对手选择哪个角色，都能有至少平分的相性。某些角色即便不选择，也不影响区间满足条件。

### 示例解释 3

没有角色对角色 \\(2\\) 具备平分或有利的相性。

 **本翻译由 AI 自动生成**