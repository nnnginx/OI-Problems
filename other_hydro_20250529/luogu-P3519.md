## 题目描述
A word consisting of $n$ lower-case letters of the English alphabet ('a'-'z') is given.

We would like to choose a non-empty contiguous (i.e. one-piece) fragment    of the word so as to maximise the difference in the number of occurrences    of the most and the least frequent letter in the fragment.

We are assuming that the least frequent letter has to occur at least once in    the resulting fragment.

In particular, should the fragment contain occurrences of only one letter,    then the most and the least frequent letter in it coincide.



## 输入格式
The first line of the standard input holds one integer $n(1\le n \le 1,000,000)$ that denotes the length of the word.

The second line holds a word consisting of $n$ lower-case letters      of the English alphabet.

In tests worth at least 30% of the points it additionally holds that $n\le 100$.


## 输出格式
The first and only line of the standard output is to hold a single integer,      equal to the maximum difference in the number of occurrences of the most      and the least frequent letter that is attained in some non-empty contiguous      fragment of the input word.


## 题目大意
给一个字符串，求其中的一段，使得出现次数最多的字符与出现次数最少的字符的出现次数之差最大。

$1 \leq N \leq 10^6$。

```input1
10
aabbaaabab
```

```output1
3
```

