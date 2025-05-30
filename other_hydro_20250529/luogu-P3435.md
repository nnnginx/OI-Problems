## 题目描述
A string is a finite sequence of lower-case (non-capital) letters of the English alphabet. Particularly, it may be an empty sequence, i.e. a sequence of 0 letters. By A=BC we denotes that A is a string obtained by concatenation (joining by writing one immediately after another, i.e. without any space, etc.) of the strings B and C (in this order). A string P is a prefix of the string !, if there is a string B, that A=PB. In other words, prefixes of A are the initial fragments of A. In addition, if P!=A and P is not an empty string, we say, that P is a proper prefix of A.


A string Q is a period of Q, if Q is a proper prefix of A and A is a prefix (not necessarily a proper one) of the string QQ. For example, the strings abab and ababab are both periods of the string abababa. The maximum period of a string A is the longest of its periods or the empty string, if A doesn't have any period. For example, the maximum period of ababab is abab. The maximum period of abc is the empty string.

Task Write a programme that:

reads from the standard input the string's length and the string itself,calculates the sum of lengths of maximum periods of all its prefixes,writes the result to the standard output.




## 输入格式
In the first line of the standard input there is one integer $k$ ($1\le k\le 1\ 000\ 000$) - the length of the string. In the following line a sequence of exactly $k$ lower-case letters of the English alphabet is written - the string.


## 输出格式
In the first and only line of the standard output your programme should write an integer - the sum of lengths of maximum periods of all prefixes of the string given in the input.


## 题目大意
对于一个仅含小写字母的字符串 $a$，$p$ 为 $a$ 的前缀且 $p\ne a$，那么我们称 $p$ 为 $a$ 的 proper 前缀。

规定字符串 $Q$ 表示 $a$ 的周期，当且仅当 $Q$ 是 $a$ 的 proper 前缀且 $a$ 是 $Q+Q$ 的前缀。若这样的字符串不存在，则 $a$ 的周期为空串。

例如 `ab` 是 `abab` 的一个周期，因为 `ab` 是 `abab` 的 proper 前缀，且 `abab` 是 `ab+ab` 的前缀。

求给定字符串所有前缀的最大周期长度之和。

```input1
8
babababa
```

```output1
24
```

