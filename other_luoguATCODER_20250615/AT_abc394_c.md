# AT_abc394_c [ABC394C] Debug

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc394/tasks/abc394_c

给定一个仅由大写字母组成的字符串 $S$。  
请输出对 $S$ 执行以下操作后得到的最终字符串：

> 只要字符串中包含连续的 `WA` 子字符串，就重复执行以下操作：
> 
> - 将字符串中首次出现的 `WA` 替换为 `AC`。

可以证明在本题的约束条件下，此操作最多只能执行有限次。

## 输入格式

输入通过标准输入按以下格式给出：

> $S$

## 输出格式

输出对 $S$ 执行题目所述操作后得到的字符串。

## 输入输出样例 #1

### 输入 #1

```
WACWA
```

### 输出 #1

```
ACCAC
```

## 输入输出样例 #2

### 输入 #2

```
WWA
```

### 输出 #2

```
ACC
```

## 输入输出样例 #3

### 输入 #3

```
WWWWW
```

### 输出 #3

```
WWWWW
```

## 说明/提示

### 约束条件

- $S$ 是长度介于 $1$ 到 $3 \times 10^5$ 之间的仅由大写字母组成的字符串

### 样例解释 1

初始字符串为 $S=$ `WACWA`。该字符串包含从第 $1$ 到 $2$ 个字符和从第 $4$ 到 $5$ 个字符的 `WA` 子字符串。第一次操作将替换最先出现的部分（即第 $1$ 到 $2$ 个字符），得到 `ACCWA`。此时字符串仅剩第 $4$ 到 $5$ 个字符的 `WA`，第二次操作替换后得到 `ACCAC`。由于 `ACCAC` 不再包含 `WA`，操作终止，因此输出 `ACCAC`。

### 样例解释 2

初始字符串为 $S=$ `WWA`。该字符串仅在第 $2$ 到 $3$ 个字符处包含 `WA`。第一次操作替换后得到 `WAC`，此时新字符串在第 $1$ 到 $2$ 个字符处出现 `WA`。第二次操作替换后得到 `ACC`。由于不再包含 `WA`，操作终止，因此输出 `ACC`。

### 样例解释 3

原始字符串 $S$ 中不包含 `WA` 子字符串，因此无需任何操作，直接输出 `WWWWW`。

翻译由 DeepSeek R1 完成