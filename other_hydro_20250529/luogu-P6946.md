## 题目描述


In typesetting, a `river` is a string of spaces formed by gaps between words that extends down several lines of text. For instance, Figure F.1 shows several examples of rivers highlighted in red (text is intentionally blurred to make the rivers more visible).

![](https://onlinejudgeimages.s3-ap-northeast-1.amazonaws.com/problem/15694/1.png)

Figure F.1 : Examples of rivers in typeset text.

Celebrated river authority Flo Ng wants her new book on rivers of the world to include the longest typographic rivers possible. She plans to set the text in a mono-spaced font (all letters and spaces have equal width) in a left-aligned column of some fixed width, with exactly one space separating words on each line (the text is not aligned on the right). For Flo, a `river` is defined as a sequence of spaces lying in consecutive lines in which the position of each space in the sequence (except the first) differs by at most $1$ from the position of the space in the line above it. Trailing white space cannot appear in a river. Words must be packed as tightly as possible on lines; no words may be split across lines. The line width used must be at least as long as the longest word in the text. For instance, Figure F.2 shows the same text set with two different line widths.

![](https://onlinejudgeimages.s3-ap-northeast-1.amazonaws.com/problem/15694/2.png)

Figure F.2 : Longest rivers $( \times )$ for two different line widths.

Given a text, you have been tasked with determining the line width that produces the longest river of spaces for that text.



## 输入格式


The first line of input contains an integer $n (2 \le n \le 2 500)$ specifying the number of words in the text. The following lines of input contain the words of text. Each word consists only of lowercase and uppercase letters, and words on the same line are separated by a single space. No word exceeds $80$ characters.



## 输出格式


Display the line width for which the input text contains the longest possible river, followed by the length of the longest river. If more than one line width yields this maximum, display the shortest such line width.



## 题目大意
#### 题目描述
在字体排印学中，“川流”是由单词之间的间隙组成的连续几列的空格。如图所示为几个用红色高亮标出的“川流”（文本被有意模糊处理来凸显川流）：

![img](https://onlinejudgeimages.s3-ap-northeast-1.amazonaws.com/problem/15694/1.png)

知名川流机构 Flo Ng 希望他在新的关于世界河流的书上出现尽可能长的川流。他会使用一种单一字宽的字体（每个字母和空格都具有相同的宽度）且左对齐，单词之间恰用一个空格分隔。对 Flo 来说，一条“川流”指的是连续几行里的空格，且相邻空格在行里出现的位置的距离不超过 $1$。川流不能包含末尾的空格。每行的单词都必须尽可能地紧凑，但不能有单词被拆到两行里。行宽至少不能短于文本中最长的一个单词。下图是同一个文本使用不同行宽的一个例子。

![img](https://onlinejudgeimages.s3-ap-northeast-1.amazonaws.com/problem/15694/2.png)

给定文本，你需要求出一个行宽使得该文本最长的川流尽可能长。

#### 输入格式
第一行有一个整数 $n(2≤n≤2500)$ 表示文本的单词个数。接下来几行为该文本的单词。每个单词都只包含大写和小写字母，且长度不超过 $80$ 个字符。

#### 输出格式
输出两个整数，分别表示使得文本出现最长的川流的行宽以及川流的长度。如果有多个行款达到川流长度的最大值，输出最小的行宽。

```input1
21
The Yangtze is the third longest
river in Asia and the longest in
the world to flow
entirely in one country

```

```output1
15 5

```

```input2
25
When two or more rivers meet at
a confluence other than the sea
the resulting merged river takes
the name of one of those rivers

```

```output2
21 6

```

## 提示
Time limit: 12 s, Memory limit: 1024 MB. 



