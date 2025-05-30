## 题目描述
Nested quotations are great not only for writing literature with a complex narrative structure, but also in programming languages. While it may seem necessary to use different quotation marks at different nesting levels for clarity, there is an alternative. We can display various nesting levels using $k$-quotations, which are defined as follows.

A $1$-quotation is a string that begins with a quote character, ends with another quote character and contains no quote characters in-between. These are just the usual (unnested) quotations. For example, 'this is a string' is a $1$-quotation.

For $k > 1$, a $k$-quotation is a string that begins with $k$ quote characters, ends with another $k$ quote characters and contains a nested string in-between. The nested string is a non-empty sequence of $(k-1)$-quotations, which may be preceded, separated, and/or succeeded by any number of non-quote characters. For example, ''All 'work' and no 'play''' is a $2$-quotation.

Given a description of a string, you must determine its maximum possible nesting level.

## 输入格式
The input consists of two lines. The first line contains an integer $n$ ($1 \le n \le 100$). The second line contains $n$ integers $a_1, a_2, \ldots , a_ n$ ($1 \le a_ i \le 100$), which describe a string as follows. The string starts with $a_1$ quote characters, which are followed by a positive number of non-quote characters, which are followed by $a_2$ quote characters, which are followed by a positive number of non-quote characters, and so on, until the string ends with $a_ n$ quote characters.

## 输出格式
Display the largest number $k$ such that a string described by the input is a $k$-quotation. If there is no such $k$, display no quotation instead.

## 题目大意
定义 $1$ 级引用是一个以引号字符 ' 开头和结尾，中间不包含引号字符的字符串。定义 $k$ 级引用为两端各有连续 $k(k>1)$ 个引号，中间有若干个 $k-1$ 级引用的字符串，其中第一个 $k-1$ 级引用前，最后一个 $k-1$ 级引用后，相邻两个 $k-1$ 级引用之间都可以添加任意个非引用字符。

现给定一个字符串中极长连续引号段的个数 $n(n\le100)$，和这 $n$ 个极长连续引号段的长度 $a_1,...,a_n$，求最大的 $k$，使得这个字符串是一个 $k$ 级引用。
若这样的 $k$ 不存在，输出 `no quotation`。

translated by @Starlight237

```input1
5
2 1 1 1 3

```

```output1
2

```

```input2
1
22

```

```output2
4

```

```input3
1
1

```

```output3
no quotation

```

## 提示
Time limit: 2000 ms, Memory limit: 1048576 kB. 

 International Collegiate Programming Contest (ACM-ICPC) World Finals 2016

