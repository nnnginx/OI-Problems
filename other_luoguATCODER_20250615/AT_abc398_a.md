# AT_abc398_a [ABC398A] Doors in the Center

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc398/tasks/abc398_a

请构造一个满足以下所有条件的长度为 $N$ 的字符串：

- 每个字符只能是 `-` 或 `=`；
- 必须是回文；
- 字符串中包含 $1$ 个或 $2$ 个 `=`。若包含 $2$ 个 `=`，则这两个 `=` 必须相邻。

可以证明，满足条件的字符串恰好存在一种。

## 输入格式

输入通过标准输入给出，格式如下：

> $N$

## 输出格式

输出满足条件的字符串。

## 输入输出样例 #1

### 输入 #1

```
4
```

### 输出 #1

```
-==-
```

## 输入输出样例 #2

### 输入 #2

```
7
```

### 输出 #2

```
---=---
```

## 说明/提示

### 约束条件

- $1 \leq N \leq 100$
- $N$ 为整数。

翻译由 DeepSeek R1 完成