# AT_code_festival_exhibition_b カッコつけ

## 题目描述

高桥君热衷于“加括号”。他喜欢在一个只由开括号 `(` 和闭括号 `)` 组成的字符串中增添或删除括号。对于每个字符串，我们定义一个称为“括号不良度”的值，它表示为了使字符串变得“完美”而必须删除的最小字符数。如果一个字符串中的括号匹配没有问题，我们称其为“完美”。特别地，空字符串也被视为“完美”。

例如，字符串 `()()(())` 是“完美”的，其“括号不良度”为 $0$。而对于 `())`，移除最后一个括号后变得“完美”，因此其“括号不良度”为 $1$。

高桥君从朋友那里得到一个字符串 $S$。他将在这个字符串中进行括号的插入或删除操作。有时，高桥君会对当前字符串一部分的“括号不良度”感到好奇。每当高桥君提出这个问题时，你需要计算并输出有关部分的“括号不良度”。

## 输入格式

输入通过标准输入给出，格式如下：

> $Q$  
> $S$  
> $x_1$ $y_1$ $z_1$  
> ...  
> $x_Q$ $y_Q$ $z_Q$

- 第一行是高桥君进行的操作（包括询问）的次数 $Q\ (1 \le Q \le 10^5)$。
- 第二行是高桥君得到的字符串 $S\ (1 \le |S| \le 10^5)$。
- 接下来的 $Q$ 行分别描述了每步操作：
  - 如果 $x_i$ 为 `(`，表示在位置 $y_i$ 插入一个开括号，此时 $z_i$ 恒为 $0$。
  - 如果 $x_i$ 为 `)`，表示在位置 $y_i$ 插入一个闭括号，此时 $z_i$ 恒为 $0$。
  - 如果 $x_i$ 为 `D`，表示删除位置 $y_i$ 的字符，此时 $z_i$ 恒为 $0$。
  - 如果 $x_i$ 为 `Q`，表示询问从位置 $y_i$ 到 $z_i$（包括 $y_i$ 和 $z_i$）间字符串的“括号不良度”。

输入保证不涉及删除或询问不存在的位置，亦不会在非法位置进行插入。所有位置索引均为从1开始计数。

## 输出格式

每次高桥君进行询问时，需输出对应的“括号不良度”结果，每个结果占一行。

### 样例解释 1

- 第 1 步操作后的字符串是 `()`
- 第 2 步操作后的字符串是 `())`
- 第 3 步操作的询问部分是 `()`，其“括号不良度”为 $0$
- 第 4 步操作后的字符串是 `(())`
- 第 5 步操作的询问部分是 `())`，其“括号不良度”为 $1$

### 样例解释 2

- 第 1 步操作后的字符串是 `((()()(()`
- 第 2 步操作后的字符串是 `(((()()(()`
- 第 3 步操作后的字符串是 `((()()(()`
- 第 4 步操作的询问部分是 `(()()`，其“括号不良度”为 $0$
- 第 5 步操作后的字符串是 `((())()(()`
- 第 6 步操作后的字符串是 `((())()()`
- 第 7 步操作的询问部分是 `((())()()`，其“括号不良度”为 $0$
- 第 8 步操作后的字符串是 `(((())()()`
- 第 9 步操作后的字符串是 `(((())())()`
- 第 10 步操作后的字符串是 `(((())()))`
- 第 11 步操作的询问部分是 `))()))`，其“括号不良度”为 $4$

 **本翻译由 AI 自动生成**

## 输入输出样例 #1

### 输入 #1

```
5
(()
D 1 0
( 3 0
Q 1 2
) 1 0
Q 2 4
```

### 输出 #1

```
0
1
```

## 输入输出样例 #2

### 输入 #2

```
11
(()()(()
( 1 0
( 1 0
D 4 0
Q 2 6
) 5 0
D 8 0
Q 1 9
( 3 0
) 8 0
D 10 0
Q 5 10
```

### 输出 #2

```
1
1
4
```