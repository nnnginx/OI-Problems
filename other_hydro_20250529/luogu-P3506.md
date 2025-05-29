## 题目描述
This task is a harder version of task Monotonicity from the third stage of 17th Polish OI. It wasn't used in the contest itself.

For an integer sequence ![](http://main.edu.pl/images/OI17/mot-en-tex.1.png) we define its monotonicity scheme as the sequence    ![](http://main.edu.pl/images/OI17/mot-en-tex.2.png) of symbols ![](http://main.edu.pl/images/OI17/mot-en-tex.3.png), ![](http://main.edu.pl/images/OI17/mot-en-tex.4.png) or ![](http://main.edu.pl/images/OI17/mot-en-tex.5.png).

The symbol ![](http://main.edu.pl/images/OI17/mot-en-tex.6.png) represents the relation between ![](http://main.edu.pl/images/OI17/mot-en-tex.7.png) and ![](http://main.edu.pl/images/OI17/mot-en-tex.8.png).

For example, the monotonicity scheme of the sequence ![](http://main.edu.pl/images/OI17/mot-en-tex.9.png) is ![](http://main.edu.pl/images/OI17/mot-en-tex.10.png).

We say that an integer sequence ![](http://main.edu.pl/images/OI17/mot-en-tex.11.png) with monotonicity scheme    ![](http://main.edu.pl/images/OI17/mot-en-tex.12.png), realizes another monotonicity scheme ![](http://main.edu.pl/images/OI17/mot-en-tex.13.png)    if for every ![](http://main.edu.pl/images/OI17/mot-en-tex.14.png) it holds that ![](http://main.edu.pl/images/OI17/mot-en-tex.15.png).

In other words, the sequence ![](http://main.edu.pl/images/OI17/mot-en-tex.16.png) can be obtained by repeating the sequence    ![](http://main.edu.pl/images/OI17/mot-en-tex.17.png) and removing appropriate suffix from that repetition.

For example, the sequence ![](http://main.edu.pl/images/OI17/mot-en-tex.18.png) realizes each and every one of the following schemes:

![](http://main.edu.pl/images/OI17/mot-en-tex.19.png)           ![](http://main.edu.pl/images/OI17/mot-en-tex.20.png)           ![](http://main.edu.pl/images/OI17/mot-en-tex.21.png)           ![](http://main.edu.pl/images/OI17/mot-en-tex.22.png)                  as well as many others.

An integer sequence ![](http://main.edu.pl/images/OI17/mot-en-tex.23.png) and a monotonicity scheme ![](http://main.edu.pl/images/OI17/mot-en-tex.24.png) are given.

Your task is to find the longest subsequence ![](http://main.edu.pl/images/OI17/mot-en-tex.25.png) (![](http://main.edu.pl/images/OI17/mot-en-tex.26.png))    of the former that realizes the latter.

## 输入格式
The first line of the standard input holds two integers ![](http://main.edu.pl/images/OI17/mot-en-tex.27.png) and ![](http://main.edu.pl/images/OI17/mot-en-tex.28.png) (![](http://main.edu.pl/images/OI17/mot-en-tex.29.png), ![](http://main.edu.pl/images/OI17/mot-en-tex.30.png)),    separated by a single space, denoting the lengths of the sequences ![](http://main.edu.pl/images/OI17/mot-en-tex.31.png) and monotonicity scheme ![](http://main.edu.pl/images/OI17/mot-en-tex.32.png) respectively.

The second input line gives the sequence ![](http://main.edu.pl/images/OI17/mot-en-tex.33.png), i.e, it holds ![](http://main.edu.pl/images/OI17/mot-en-tex.34.png) integers ![](http://main.edu.pl/images/OI17/mot-en-tex.35.png) separated by single spaces (![](http://main.edu.pl/images/OI17/mot-en-tex.36.png)).

Finally, the third lines gives the monotonicity scheme ![](http://main.edu.pl/images/OI17/mot-en-tex.37.png), i.e., it holds ![](http://main.edu.pl/images/OI17/mot-en-tex.38.png) s…


## 输出格式
In the first line of the standard output your program should print out a single integer ![](http://main.edu.pl/images/OI17/mot-en-tex.40.png),    the maximum length of a subsequence of ![](http://main.edu.pl/images/OI17/mot-en-tex.41.png) that realizes the scheme ![](http://main.edu.pl/images/OI17/mot-en-tex.42.png).

In the second line it should print out any such subsequence ![](http://main.edu.pl/images/OI17/mot-en-tex.43.png), separating its elements by single spaces.


## 题目大意
### 题目描述

本题是来自 POI 2010 第三阶段的[单调性](https://www.luogu.com.cn/problem/P3541)一题的加强版，但并没有在那次比赛中被使用。

**译自 POI 2010 「[Monotonicity 2](https://szkopul.edu.pl/problemset/problem/0_pcwjQ6no8LDss0IWNLbb2_/site/?key=statement)」**

对于一个整数序列 $a_1, a_2, ..., a_n$，我们定义其“单调序列"为一个由 $<$，$>$ 和 $=$ 组成的符号序列 $s_1, s_2, ... s_{n-1}$，其中符号 $s_i$ 表示 $a_i$ 和 $a_{i+1}$ 之间的关系。例如，数列 $2, 4, 3, 3, 5, 3$ 的单调序列为 $<, >, =, <, >$。

对于整数序列 $b_1, b_2, ..., b_{n+1}$ 以及其单调序列 $s_1, s_2, ..., s_n$，如果符号序列 $s_1', s_2', ..., s_k'$ 满足对所有 $1 \le i \le n$ 有 $s_i = s_{((i - 1) \bmod n) + 1}'$，我们就说序列 $s_1, s_2, ..., s_n$ 「实现」了序列 $s_1', s_2', ..., s_k'$。也就是说，序列 $s_1, s_2, ..., s_n$ 可以通过重复多次 $s_1', s_2', ..., s_k'$ 序列并删除一个后缀得到。例如，整数数列 $2, 4, 3, 3, 5, 3$ 至少实现了以下符号序列：
* $<, >, =$
* $<, >, =, <, >$
* $<, >, =, <, >, <, <, =$
* $<, >, =, <, >, =, >, >$

给定一个整数序列 $a_1, a_2, ..., a_n$ 以及一个单调序列 $s_1, s_2, ..., s_k$，求出原整数序列最长的子序列 $a_{i_1}, a_{i_2}, ..., a_{i_m} (1 \le i_1 \lt i_2 \lt ... \lt i_m \le n)$ 使得前者的单调序列实现后者的符号序列。

### 输入格式

第一行包含用空格分隔的两个整数 $n,k$，分别表示整数序列 $(a_i)$ 的长度和单调序列 $(s_j)$ 的长度。

第二行包含用空格分隔的 $n$ 个整数，表示序列 $a_i$.

第三行包含用空格分隔的 $k$ 个符号，表示符号序列 $s_j$.

### 输出格式

第一行输出一个整数 $m$，表示序列 $a_1, a_2, ..., a_n$ 的最长的「实现」了单调序列 $s_1, s_2, ..., s_n$ 的子序列。

第二行输出任意一个这样的子序列 $a_{i_1}, a_{i_2}, ..., a_{i_n}$，元素之间用空格分隔。

### 数据范围

对于 $100\%$ 的数据， $1 \le n \le 500000,1 \le k \le 500000 , 1 \le a_i \le 1000000 , s_j \in \{<, >, =\}$ 。

感谢 [本帖](https://www.luogu.com.cn/discuss/67056) 提供的 SPJ。翻译来自于 [LibreOJ](https://loj.ac/p/3009)。

```input1
7 3
2 4 3 1 3 5 3
< > =
```

```output1
6
2 4 3 3 5 3
```

