## 题目背景
Pareidolia is the phenomenon where your eyes tend to see familiar patterns in
images where none really exist -- for example seeing a face in a cloud.  As you
might imagine, with Farmer John's constant proximity to cows, he often sees
cow-related patterns in everyday objects.  For example, if he looks at the
string "bqessiyexbesszieb", Farmer John's eyes ignore some of the letters and
all he sees is "bessiexbessieb" -- a string that has contains two contiguous
substrings equal to "bessie". 

## 题目描述
Given a string of length at most $2\cdot 10^5$ consisting only of characters
a-z, where each character has an associated deletion cost, compute the maximum
number of contiguous substrings that equal "bessie" you can form by deleting
zero or more characters from it, and the minimum total cost of the characters you need to
delete in order to do this.

## 输入格式
The first line contains the string. The second line contains the deletion cost
associated with each character (an integer in the range $\left[1,1000\right]$).

## 输出格式
The maximum number of occurrences, and the minimum cost to produce this number
of occurrences.

## 题目大意
### 题目背景

Pareidolia 是一种现象，指的是人们倾向于在并不真正存在的地方看到熟悉的图案——例如在云中看到一张脸。可以想象，由于农夫 John 经常与奶牛接触，他常常在日常物品中看到与奶牛相关的图案。例如，如果他看到字符串 "bqessiyexbesszieb"，农夫 John 的眼睛会忽略其中的一些字母，而他看到的只是 "bessiexbessieb"——一个包含两个连续子串等于 "bessie" 的字符串。

### 题目描述

给定一个长度不超过 $2 \cdot 10^5$ 的字符串，且仅由字符 a-z 组成，其中每个字符都有一个相关的删除成本。计算通过删除零个或多个字符后，能够形成的等于 "bessie" 的连续子串的最大数量，以及为了实现这一目标所需删除字符的最小总成本。

### 输入格式

第一行包含字符串。第二行包含每个字符的删除成本（一个在 $\left[1,1000\right]$ 范围内的整数）。

### 输出格式

输出最大数量的 "bessie" 出现次数，以及实现这一数量所需的最小成本。

### 提示

对于第一个样例，通过删除位置 4 的 's'，我们可以使整个字符串变为 "bessie"。位置 4 的字符成本为 $4$，因此我们的答案是成本 $4$ 得到 $1$ 个 "bessie"，这是我们可以做到的最佳结果。

对于第二个样例，通过删除位置 5-7 的 "con"，我们可以使字符串变为 "bebessiete"，其中包含中间的 "bessie"。位置 5-7 的字符成本为 $5 + 7 + 9 = 21$，因此我们的答案是成本 $21$ 得到 $1$ 个 "bessie"，这是我们可以做到的最佳结果。

对于第三个样例，通过删除位置 4-10 的 "giraffe"，我们可以使字符串变为 "bessiebessibessie"，其中包含开头和结尾的 "bessie"。"giraffe" 有 7 个字符，且所有字符的成本均为 $1$，因此我们的答案是成本 $7$ 得到 $2$ 个 "bessie"，这是我们可以做到的最佳结果。此样例满足第二个子任务的约束条件。

- 输入 4-5：$N \le 2000$。
- 输入 6-8：所有成本均为 $1$。
- 输入 9-17：没有额外限制。

```input1
besssie
1 1 5 4 6 1 1

```

```output1
1
4

```

```input2
bebesconsiete
6 5 2 3 6 5 7 9 8 1 4 5 1

```

```output2
1
21

```

```input3
besgiraffesiebessibessie
1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1

```

```output3
2
7

```

## 提示
For the first sample, by deleting the 's' at position 4 we can make the whole string "bessie". The
character at position 4 has a cost of $4$, so our answer is cost $4$ for $1$
instance of "bessie", which is the best we can do.

For the second sample, by deleting the "con" at positions 5-7, we can make the string "bebessiete"
which has "bessie" in the middle. Characters 5-7 have costs $5 + 7 + 9 = 21$, so
our answer is cost $21$ for $1$ instance of "bessie", which is the best we can
do.

For the third sample, by deleting the "giraffe" at positions 4-10, we can make the string
"bessiebessibessie", which has "bessie" at the beginning and the end. "giraffe"
has 7 characters and all characters have cost $1$, so our answer is cost $7$ for
$2$ instances of "bessie", which is the best we can do. This sample satisfies the constraints for the second subtask.

- Inputs 4-5: $N\le 2000$.
- Inputs 6-8: All costs are $1$.
- Inputs 9-17: No additional constraints.

