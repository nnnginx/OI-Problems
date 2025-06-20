# AT_agc044_f [AGC044F] Name-Preserving Clubs

## 题目描述

你面前有 $N$ 个名字各不相同的人和 $K$ 个俱乐部。已知每个俱乐部的完整成员列表（即 $K$ 个无序集合）。一个人可以同时参加多个俱乐部，也可以不参加任何俱乐部。多个俱乐部可能拥有相同的成员集合。此处，$K$ 是满足以下条件的最小值：

- 若这 $N$ 个人全部改掉名字（但名字仍需各不相同），并给你 $K$ 个俱乐部改名后成员的名单（不告诉你哪个名单对应哪个俱乐部），你必须能够准确地推断出每个改名后的人对应的原名。

你的任务是计算出这样的俱乐部成员构成方式有多少种。如果超过 $1000$ 种，请输出 $-1$。

需要注意的是，如果存在一种重命名方式可以从一种成员构成转变为另一种，那么它们被认为是相同的。

### 输入格式

输入为一个整数 $N$，表示人数。

### 输出格式

输出满足条件的成员构成的数量。如果数量超过 $1000$ 种，则输出 $-1$。

### 数据范围

- $2 \le N \le 2 \cdot 10^{18}$

### 示例说明

1. 当 $K$ 为 $1$ 时，唯一的构成为 $\{\{1\}\}$，$\{\{2\}\}$ 被视为与其相同。

2. 当 $K$ 为 $2$ 时，唯一的构成为 $\{\{1\}, \{1, 2\}\}$。

3. 当 $K$ 为 $3$ 时，有多个不同的构成，例如：
   - $\{\{1\}, \{2\}, \{1, 3\}\}$
   - $\{\{1\}, \{1, 2\}, \{2, 3\}\}$
   - 其他诸如 $\{\{1, 2\}, \{1, 3\}, \{1, 2, 4\}\}$ 等。

这些示例旨在帮助理解何为不同的成员构成及如何计算。

 **本翻译由 AI 自动生成**

## 输入格式

无

## 输出格式

无

## 输入输出样例 #1

### 输入 #1

```
2
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
3
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
4
```

### 输出 #3

```
7
```

## 输入输出样例 #4

### 输入 #4

```
13
```

### 输出 #4

```
6
```

## 输入输出样例 #5

### 输入 #5

```
26
```

### 输出 #5

```
-1
```

## 输入输出样例 #6

### 输入 #6

```
123456789123456789
```

### 输出 #6

```
-1
```