# AT_discovery_2016_final_c 特別講演「括弧列と塗り分け」

## 题目描述

你是一位讲授特别课程「括号序列与涂色」的讲师。今天，你计划向学生们介绍一种为含有 `(` 和 `)` 的字符串 $S$ 涂色的方法。字符串 $S$ 已经保证了括号的配对关系是正确无误的。

我们要为 $S$ 中的每个字符涂上红色或蓝色。如果第 $i$ 个 `(` 和第 $j$ 个 `)` 是配对的，则要求子串 $S[i, j]$ 中，红色字符计数为 $R$，蓝色字符计数为 $B$，需要满足 $|R - B| \leq K$。

请计算出满足条件的所有涂色方案的总数，然后将结果对 $1,000,000,007$ 取模，并输出。

对于本问题，括号配对正确的字符串定义如下：

1. 空字符串视作配对正确。
2. 如果 $A$ 和 $B$ 都是配对正确的字符串，那么 $AB$ 也是配对正确的。
3. 若 $A$ 是配对正确的字符串，则形式为 `(`$A$`)` 的字符串也是配对正确的，并且括号 `(` 与 `)` 视为一对。
4. 不满足上述条件的字符串即为配对错误的。

## 输入格式

输入如下：

- 第一行是括号字符串 $S$，其长度满足 $2 \leq |S| \leq 3,000$，且 $S$ 配对正确。
- 第二行是整数 $K\ (0 \leq K \leq 3,000)$，表示涂色时的约束。

## 输出格式

输出满足条件的涂色方案的个数，并对 $1,000,000,007$ 取模。

## 输入输出样例 #1

### 输入 #1

```
()()
0
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
()()
2
```

### 输出 #2

```
16
```

## 输入输出样例 #3

### 输入 #3

```
(()())
2
```

### 输出 #3

```
50
```

## 输入输出样例 #4

### 输入 #4

```
()()()()()()()()()()()()()()()()
2
```

### 输出 #4

```
294967268
```

## 说明/提示

### 部分分数

本题设有部分得分。

- 若能正确解决满足 $2 \leq |S| \leq 8$ 条件的数据集，可得 $10$ 分。
- 解决 $2 \leq |S| \leq 100$ 数据集，可得 $10$ 分的额外奖励。
- 满足完整数据集的要求，可以额外获得 $50$ 分，总计 $70$ 分。

### 示例解释

1. 在示例 1 中，第 $1$ 和第 $2$ 个字符，$3$ 和第 $4$ 个字符分别配对。可能的涂色情况有：`<><>`, `<>[]`, `[><]`, `[[]]` 共 $4$ 种。
2. 在示例 2 中，共有 $16$ 种涂色方案。
3. 在示例 3 中，多个配对存在。
4. 示例 4 的涂色方案总数为 $4,294,967,296$，输出其对 $1,000,000,007$ 取模结果 $294,967,268$。

 **本翻译由 AI 自动生成**