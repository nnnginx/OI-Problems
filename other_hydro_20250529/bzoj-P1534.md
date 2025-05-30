## 题意翻译

斐波那契数是一个这样定义的整数：$F(0)=1$，$F(1)=1$，$F(i)=F(i-1)+F(i-2)$ $(2 \le i)$，前几个数是这样的 $1, 1, 2, 3, 5, 8, \ldots$

伟大的计算机学家 Byteazar 正在做一个非凡的计算机，其中的数由斐波那契表示！

如一个数列 $b_1, b_2, \ldots , b_n$ 表示数字 $F(1) \times b_1+b_2 \times F(2)+ \ldots +b_n \times F(n)$（不使用 $F(0)$ ）。

不幸的是，这样的表示并不明确，即相同的数字可以有不同的表示。比如 $42$ 可以表示为 $(0,0,0,0,1,0,0,1)$，$(0,0,0,0,1,1,1,0)$ 或 $(1,1,0,1,0,1,1)$，于是 Byteazar 加了一个限制：

- 如果 $n>1$，那么$b_n=1$，即数字的表示不包含前导零。

- 如果 $b_i=1$，那么 $b_{i+1}=0$，即数字的表示不包含两个（或多个）连续的数字。

这个计算机的建设比 Byteazar 所认为的要难，现在请你来帮帮他~。

你需要写一个程序：

读取两个正整数的表示，计算并向标准输出写入其和的表示。

输入格式：

输入的第一行先是一个正整数，为 $x$ 的斐波那契表示的长度，接下来的序列是 $x$ 的斐波那契表示。

第二行的第一个数字也是一个正整数，为 $y$ 的斐波那契表示的长度，接下来的序列是 $y$ 的斐波那契表示。

输出格式：输出只有一行程序，应写入$x+y$ 的和的斐波纳契表示（满足上述条件），同样是先输出一个正整数 $n$ ，表示 $x+y$ 的和的斐波纳契表示的长度，然后再输出 $x+y$ 的和的斐波那契表示。

$1\leq n \leq 10^6$

## 题目描述

Fibonacci numbers are an integer sequence defined in the following way: $Fib_0=1$, $Fib_1=1$, $Fib_i=Fib_{i-1}+Fib_{i-2}$ (for $i\ge 2$). The first few numbers in this sequence are: ($1,1,2,3,5,8,\cdots$).

The great computer scientist Byteazar is constructing an unusual computer, in which numbers are represented in Fibonacci system i.e. a bit string $(b_1,b_2,\cdots,b_n)$ denotes the number $b_1\cdot Fib_1+b_2\cdot Fib_2+\cdots+b_n\cdot Fib_n$. (Note that we do not use $Fib_0$.) Unfortunately, such a representation is ambiguous i.e. the same number can have different representations. The number $42$, for instance, can be written as: $(0,0,0,0,1,0,0,1)$, $(0,0,0,0,1,1,1,0)$ or $(1,1,0,1,0,1,1)$. For this very reason, Byteazar has limited himself to only using representations satisfying the following conditions:

if $n>1$, then $b_n=1$, i.e. the representation of a number does not contain leading zeros.

if $b_i=1$, then $b_{i+1}=0$ (for $i=1,\cdots,n-1$), i.e. the representation of a number does not contain two (or more) consecutive ones.

The construction of the computer has proved more demanding than Byteazar supposed. He has difficulties implementing addition. Help him!

TaskWrite a programme which:

reads from the standard input the representations of two positive integers,calculates and writes to the standard output the representation of their sum.

## 输入格式

The input contains the Fibonacci representations (satisfying the aforementioned conditions) of two positive integers $x$ and $y$ - one in the first, the other in the second line. Each of these representations is in the form of a sequence of non-negative integers, separated by single spaces. The first number in the line denotes the length of the representation $n$, $1\le n\le 10^6$. It is followed by $n$ zeros and/or ones.

输入的第一行先是一个正整数，为 $x$ 的斐波那契表示的长度，接下来的序列是 $x$ 的斐波那契表示。

第二行的第一个数字也是一个正整数，为 $y$ 的斐波那契表示的长度，接下来的序列是 $y$ 的斐波那契表示。

## 输出格式

In the first and only line of the output your programme should write the Fibonacci representation (satisfying the aforementioned conditions) of the sum $x+y$. The representation should be in the form of a sequence of non-negative integers, separated by single spaces, as it has been described in the Input section. The first number in the line denotes the length of the representation $n$, $1\le n\le 10^6$. It is followed by $n$ zeros and/or ones.

输出只有一行程序，应写入 $x+y$ 的和的斐波纳契表示（满足上述条件），同样是先输出一个正整数 $n$，表示 $x+y$ 的和的斐波纳契表示的长度，然后再输出 $x+y$ 的和的斐波那契表示。

保证输入输出的数据长度都不大于 $10^6$ 也不小于 $1$;

## 输入样例
```plain
4 0 1 0 1
5 0 1 0 0 1
```


## 输出样例
```plain
6 1 0 1 0 0 1
```