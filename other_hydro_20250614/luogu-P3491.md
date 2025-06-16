## 题目描述
Let $h$ be a function acting on strings composed of the digits 0 and 1. The function $h$ transforms the string $w$ by replacing (independently and concurrently) every digit 0 with 1 and every digit 1 with the string "10". For example $h("1001") = "101110"$, $h("") = ""$ (i.e. $h$ assigns an empty string to the empty string). Note that $h$ is an injection, or a one - to - one function. By $h^k$ we denote the function $h$ composed with itself $k$ times. In particular, $h^0$ is the identity function $h^0(w)=w$.

We are interested in the strings of the form $h^k("0")$ for $k = 0,1,2,3,\cdots$. This sequence begins with the following strings:

"0", "1", "10", "101", "10110", "10110101".

We call the string $x$ a substring of the string $y$ if it occurs in $y$ as a contiguous (i.e. one - block) subsequence. A sequence of integers $k_1,k_2,\cdots,k_n$ is given. Your task is to check whether a string of the form $h^{k_1}("0") \cdot h^{k_2}("0") \cdots h^{k_n}("0")$ is a substring of $h^m("0")$ for some $m$.

## 输入格式
The first line of the standard input contains a single integer $t$, $1 \leq t \leq 13$, denoting the number of test units. The first line of each test unit's description contains one integer $n$, $1 \leq n \leq 100000$. The second line of each description holds $n$ non - negative integers $k_1,k_2,\cdots,k_n$, separated by single spaces. The sum of the numbers in the second line of any test unit description does not exceed 10000000.

## 输出格式
Your programme should print out $t$ lines to the standard output, one for each test unit. Each line corresponding to a test unit should contain one word: TAK (yes in Polish - if $h^{k_1}("0") \cdot h^{k_2}("0") \cdots h^{k_n}("0")$ is a substring of $h^m("0")$ for some $m$ in that test unit, or NIE (no in Polish) otherwise. 

## 题目大意
## 题目描述

函数  $h$ 作用于由数字  $0$ 和  $1$ 组成的字符串，其通过将每一个数字  $0$ 替换为  $1$，将每一个数字  $1$ 替换为字符串  $10$ 来独立且同时地变换字符串  $w$。

例如：

 $$h(``1001")=``101110"$$
 $$h(``\ ")=``\ "$$

其中例二即把空字符串赋值给空字符串。

注意， $h$ 是一个一对一的函数。

我们用  $h^k$ 表示函数  $h$ 使用  $k$ 次。

特别的， $h^0(w)=w$。 

我们对  $k = 0, 1, 2, ...$ 的  $h^k(``0")$ 形式的字符串感兴趣，这个序列为:

 $$ ``0", ``1", ``10", ``101", ``10110", ``10110101", \ldots $$

如果字符串  $x$ 在  $y$ 中以一个连续的（即一个块）子串出现，我们就称  $x$ 为字符串  $y$ 的子串。给出整数  $k_1, k_2, k_3, ..., k_n $ 的序列。你的任务是检查是否有  $m$ ，使 $h^{k_1}(``0") \cdot h^{k_2}(``0") \cdot \ldots \cdot h^{k_n}(``0") $ 形式的字符串是  $h^m(``0")$ 的子串。 

## 输入内容
输入的第一行包含一个整数  $t$ 表示样例数，  $1 \leq t \leq 13$。每个样例输入两行，一行  $n$ ， $1 \leq n \leq 100000$ ，另一行为  $n$ 个非负整数  $k_1, k_2, k_3, ..., k_n $，用单个空格分隔。

## 输出内容
您的程序应该输出  $t$ 行，每个测试输出一行。如果存在  $m$ 使  $h^{k_1}(``0") \cdot h^{k_2}(``0") \cdot \ldots \cdot h^{k_n}(``0") $ 是  $h^m(``0")$ 的子串，就输出 `TAK`（波兰语中的 _yes_ ），如果不存在  $m$，则输出 `NIE`（波兰语中的 _no_ ）。

_Translated By in\_young\_ren_ 

```input1
2
2
1 2
2
2 0

```

```output1
TAK
NIE

```

