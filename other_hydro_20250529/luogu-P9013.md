## 题目描述
Bessie is using the latest and greatest innovation in text-editing software, miV! She starts with an input string consisting solely of upper and lowercase English letters and wishes to transform it into some output string. With just one keystroke, miV allows her to replace all occurrences of one English letter $c_1$ in the string with another English letter $c_2$. For example, given the string `aAbBa`, if Bessie selects $c_1$ as `a` and $c_2$ as `B`, the given string transforms into `BAbBB`.

Bessie is a busy cow, so for each of $T
(1 \le T \le 10)$ independent test cases, output the minimum number of keystrokes required to transform her input string into her desired output string. 

## 输入格式
The first line contains $T$, the number of independent test cases.

The following $T$ pairs of lines contain an input and output string of equal length. All characters are upper or lowercase English letters (either `A` through `Z` or `a` through `z`). The sum of the lengths of all strings does not exceed $10^5$. 

## 输出格式
For each test case, output the minimum number of keystrokes required to change the input string into the output string, or $−1$ if it is impossible to do so. 

## 题目大意
### 题目描述

Bessie 正在使用世界上最先进最伟大的文本编辑器：miV！她想将一个仅由大写和小写英文字母组成的字符串转换为一个新的字符串。每一次操作，miV 可以将字符串中所有的字母  $c_1$ 替换成另一种字母 $c_2$。例：对于字符串`aAbBa`, 如果将其中的 `a` 替换成 `B`, 那么字符串会变为`BAbBB`。

Bessie 非常地忙碌, 所以对于给出的 $T
(1 \le T \le 10)$ 组测试数据, 请输出她至少需要多少次操作才能把原字符串转换为新字符串。

### 输入格式

第一行是一个整数 $T$, 表示测试数据的数量。

接下来有 $T$ 对长度相等的字符串。字符串中所有的字符都是大写或小写的字母。字符串的长度不会超过 $10^5$。

### 输出格式

对于每组测试数据，输出转换字符串需要的最小操作数。

如果这不可能做到，输出 $-1$。

### 样例 1 解释

第一组数据：两个字符串相等，所以不需要任何操作。

第二组数据：你不可能在把其中一个 `B` 转换为 `A`的同时保持剩下一个 `B` 不变。

第三组数据：你可以把字符串中所有的 `a` 转换为 `b`。

第四组数据：你可以按 $\texttt{ABCD} \rightarrow \texttt{EBCD} \rightarrow \texttt{EACD} \rightarrow \texttt{BACD}$ 的方式转换。

### 数据范围

 - 对于 $ 40 \% $ 的数据，字符串的长度不超过 $50$。
 - 对于另外 $ 20\% $ 的数据，所有的字符串仅包含从 `a` 到 `e` 的小写字母。
 - 对于 $ 100\% $ 的数据，字符串的长度不超过 $10^5$，$1 \le T \le 10$。

```input1
4
abc
abc
BBC
ABC
abc
bbc
ABCD
BACD
```

```output1
0
-1
1
3
```

## 提示
### Explanation for Sample 1

The first input string is the same as its output string, so no keystrokes are required.

The second input string cannot be changed into its output string because Bessie cannot change one `B`' to `A` while keeping the other as `B`.

The third input string can be changed into its output string by changing `a` to `b`.

The last input string can be changed into its output string like so: $\texttt{ABCD} \rightarrow \texttt{EBCD} \rightarrow \texttt{EACD} \rightarrow \texttt{BACD}$.

### Scoring

 - Inputs $2-6$: Every string has a length at most $50$.
 - Inputs $7-9$: All strings consist only of lowercase letters `a` through `e`
 - Inputs $10-15$: No additional constraints.

