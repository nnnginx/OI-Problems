## 题目描述
Farmer John's farm is in the shape of an $N \times N$ grid of fields ($1 \le N \le 500$), each labeled with a letter in the alphabet.  For example:

```cpp
ABCD
BXZX
CDXB
WCBA
```
Each day, Bessie the cow walks from the upper-left field to the lower-right field, each step taking her either one field to the right or one field downward. Bessie keeps track of the string that she generates during this process, built from the letters she walks across. She gets very disoriented, however, if this string is a palindrome (reading the same forward as backward), since she gets confused about which direction she had walked. Please help Bessie determine the number of distinct routes she can take that  correspond to palindromes. Different ways of obtaining the same palindrome count multiple times. Please print your answer modulo 1,000,000,007.

## 输入格式
The first line of input contains $N$, and the remaining $N$ lines contain the $N$ rows of the grid of fields. Each row contains $N$ characters that are in the range A..Z.

## 输出格式
Please output the number of distinct palindromic routes Bessie can take, modulo 1,000,000,007.

## 题目大意
### 题目描述

Farmer John 的农场是一个 $N \times N$ 的网格（$1 \le N \le 500$），每个格子标有一个字母。例如：

```
ABCD
BXZX
CDXB
WCBA
```

每天，奶牛 Bessie 从左上角的格子走到右下角的格子，每一步只能向右或向下移动一个格子。Bessie 会记录下她走过的路径所生成的字符串，这个字符串由她经过的格子上的字母组成。然而，如果这个字符串是一个回文串（即正读和反读相同），她会感到非常困惑，因为她会分不清自己走过的方向。请帮助 Bessie 计算她可以走的不同路径中，对应回文串的数量。即使生成相同回文串的方式不同，也需要分别计数。请输出答案对 1,000,000,007 取模的结果。

### 输入格式

输入的第一行包含 $N$，接下来的 $N$ 行包含网格的 $N$ 行。每行包含 $N$ 个字符，字符范围为 A..Z。

### 输出格式

请输出 Bessie 可以走的不同回文路径的数量，对 1,000,000,007 取模。

### 说明/提示

Bessie 可以生成以下回文串：

- 1 个 "ABCDCBA"
- 1 个 "ABCWCBA"
- 6 个 "ABXZXBA"
- 4 个 "ABXDXBA"

```input1
4
ABCD
BXZX
CDXB
WCBA
```

```output1
12
```

## 提示
Bessie can make the following palindromes

1 x "ABCDCBA"

1 x "ABCWCBA"

6 x "ABXZXBA"

4 x "ABXDXBA"


