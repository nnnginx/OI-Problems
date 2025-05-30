## 题目描述


In computing, regular expressions is a powerful tool for text search and string matching. In this problem a simplified version of regular expressions is used:

- An empty string ` ` is a regular expression, only the empty string matches it.

- A single lowercase letter `c` is a regular expression, a string consisting of a single letter $c$ matches it.

- A dot `.` is a regular expression, a string consisting of any single letter matches it.

- Alternation: if $α$ and $β$ are regular expressions then `(α|β)` is a regular expression, a string $s$ matches it only if $s$ matches $α$ or $s$ matches $β$.

- Concatenation: if $α$ and $β$ are regular expressions then `(αβ)` is a regular expression, a string $s$ matches it only if $s =$ `xy`, $x$ matches $α$ and $y$ matches $β$.

- Kleene star: if $α$ is regular expression then `(α∗)` is a regular expression, a string $s$ matches it only if $s$ is empty or $s =$ `xy`, $x$ is nonempty and matches $α$ and $y$ matches $(α∗).$ In other words, $s$ consists of zero or more strings, each of them matches $α.$

Parentheses can be omitted, in this problem Kleene star has the highest priority, concatenation has medium priority and alternation has lowest priority. Thus `abc*|de` means `(ab(c*))|(de)`.

For example, string `abcabcab` matches `a(bc|a)*ab`, but string `abcbab` does not.

Your task is to find the shortest string that matches the given regular expression $E$ and contains the given substring $S$ .



## 输入格式


The first line of the input file contains the regular expression $E$ . The second line of the input file contains the substring $S (1 \le |E| , |S| \le 10 000)$ .

String $S$ consists of lowercase English letters. Expression $E$ consists of lowercase English letters and special characters: dots (`.`), parentheses (`(`) and (`)`), pipes (`|`), and asterisks (`*`).



## 输出格式


Output the shortest possible string $T$ that both matches $E$ and contains $S$ as substring. If there are no such strings, output `NO`.

The string $T$ should contain only lowercase English letters.



## 题目大意
在计算机中，正则表达式是文本搜索和字符串匹配的强力工具。这道题将使用简化后的正则表达式：

+ 一个空字符串()是一个正则表达式，且只有空字符串匹配它。

+ 一个小写字母(c)是一个正则表达式，只有仅包含一个字母 $c$ 的字符串匹配它。

+ 点(.)是一个正则运算符，任何仅包含一个字母的字符串都匹配它。

+ 或运算：若 $\alpha$ 和 $\beta$ 是正则表达式，则 ( $\alpha$ | $\beta$ ) 是正则表达式；当且仅当字符串 $s$ 匹配 $\alpha$ 或 匹配 $\beta$ 时，$s$ 匹配 ( $\alpha$ | $\beta$ )。

+ 与运算：若 $\alpha$ 和 $\beta$ 是正则表达式，则 ( $\alpha\beta$ ) 是正则表达式；当且仅当字符串 $s$ 可以分为两个子串 $x$ 和 $y$ ，且 $x$ 匹配 $\alpha$ ，$y$ 匹配 $\beta$ 时，$s$ 匹配 ( $\alpha\beta$ )。

+ 星号运算：若 $\alpha$ 是正则表达式，则 ( $\operatorname{\alpha_*}$ ) 是正则表达式；当且仅当字符串 $s$ 为空或 $s$ 可以被分为若干个匹配 $\alpha$ 的子串时，$s$ 匹配 ( $\operatorname{\alpha_*}$ )。

在本题中，括号可以被省略；运算符的优先级从高到低依次为：星号运算、与运算，或运算。所以 ( $abc_*$ | $de$ ) 即 ( $ab$ ( $c_*$ )) | ( $de$ ) 。

举个例子，字符串 $abcabcab$ 匹配 ( $a$ ( $bc$ | $a$ )$_*ab$ )，而字符串 $abcbab$ 并不匹配它。

现给定正则表达式 $E$ 和字符串 $S$ ，要求找出最短的匹配 $E$ 的字符串 $T$ ，且 $T$ 必须包含 $S$ 。

```input1
a.*b
bab

```

```output1
abab

```

```input2
(ab)*
bb

```

```output2
NO

```

## 提示
Time limit: 10 s, Memory limit: 256 MB. 



