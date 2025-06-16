## 题目背景
**Note: The time limit for this problem is 4s, 2x the default.**

Pareidolia is the phenomenon where your eyes tend to see familiar patterns in
images where none really exist -- for example seeing a face in a cloud.  As you
might imagine, with Farmer John's constant proximity to cows, he often sees
cow-related patterns in everyday objects.  For example, if he looks at the
string "bqessiyexbesszieb", Farmer John's  eyes ignore some of the letters and
all he sees is "bessiebessie".  

## 题目描述
Given a string $s$, let $B(s)$ represent the maximum number of repeated copies
of "bessie" one can form by deleting zero or more of the characters from $s$. 
In the example above, $B(\text{``bqessiyexbesszieb"}) = 2$.

Computing $B(s)$ is an interesting challenge, but Farmer John is interested in
solving a challenge that is even more interesting: Given a string $t$ of length
at most $3\cdot 10^5$ consisting only of characters a-z, compute the sum of
$B(s)$ over all contiguous substrings $s$ of $t$.

## 输入格式
The input consists of a nonempty string of length at most $3\cdot 10^5$ whose
characters are all lowercase English letters.

## 输出格式
Output a single number, the total number of bessies that can be made across all
substrings of the input string.

## 题目大意
### 题目背景

**注意：本题的时间限制为 4 秒，是默认时间限制的 2 倍。**

Pareidolia 是一种现象，指的是人们倾向于在并不真正存在的地方看到熟悉的图案——例如在云中看到一张脸。可以想象，由于农夫 John 经常与奶牛接触，他常常在日常物品中看到与奶牛相关的图案。例如，如果他看到字符串 "bqessiyexbesszieb"，农夫 John 的眼睛会忽略其中的一些字母，而他看到的只是 "bessiebessie"。

### 题目描述

给定一个字符串 $s$，令 $B(s)$ 表示通过删除 $s$ 中的零个或多个字符后，能够形成的 "bessie" 的最大重复次数。在上面的例子中，$B(\text{``bqessiyexbesszieb"}) = 2$。

计算 $B(s)$ 是一个有趣的挑战，但农夫 John 对解决一个更有趣的挑战感兴趣：给定一个长度不超过 $3 \cdot 10^5$ 的字符串 $t$，且仅由字符 a-z 组成，计算所有连续子串 $s$ 的 $B(s)$ 之和。

### 输入格式

输入由一个非空字符串组成，长度不超过 $3 \cdot 10^5$，且所有字符均为小写英文字母。

### 输出格式

输出一个数字，表示输入字符串的所有子串中能够形成的 "bessie" 的总数。

### 提示

对于第一个样例，有 12 个子串恰好包含 $1$ 个 "bessie"，有 $1$ 个子串恰好包含 $2$ 个 "bessie"，因此总数为 $12 \cdot 1 + 1 \cdot 2 = 14$。

- 输入 3-5：字符串长度不超过 $5000$。
- 输入 6-12：没有额外限制。

```input1
bessiebessie

```

```output1
14

```

```input2
abcdefghssijebessie

```

```output2
28

```

## 提示
For the first sample, twelve substrings contain exactly $1$ "bessie", and $1$ string contains exactly $2$ "bessie"s, so the total is $12\cdot 1+1\cdot 2=14$.

- Inputs 3-5: The string has length at most $5000$.
- Inputs 6-12: No additional constraints.

