## 题目描述

John and Brus are freshmen at the primary school．Their first home task is to learn some integer numbers．It is not so hard for the guys and they decide to impress their teacher by learning all lucky numbers between $A$ and $B$．inclusive．

As you already know from the previous year contest $4$ and $7$ are lucky digits，and all the other digits are not lucky．A lucky number is a number that contains only lucky digits in decimal notation．

After learning all lucky numbers in $[A,B]$ range John and Brus still have some free time and now they decide to learn additionally each lucky number $N$ that is out of $[A,B]$ range，but the reversed number of $N$ is in this range．Here reversed number of $N$ is the number $N$ written in decimal notation，but the order of digits is reversed．For example，the reversed number of $447$ is $744$ and reversed number of $774474444$ is $444474477$．

You are given integers $A$ and $B$ and your task is to find the total number of lucky numbers learned by John and Brus．

## 输入格式

**本题有多组数据**

The first line contains single integer $T$ － the number of test cases．Each test case consists of a single line containing two integers $A$ and $B$ separated by a single space．

## 输出格式

For each test case print a single line containing the total number of lucky numbers learned by John and Brus．

```input1
2 
1 100
44 47
```

```output1
6
3
```

## 数据规模与约定

$100\%$ 的数据满足：$1 \le T \le 74$，$1 \le A \le B \le 10^{50}$。

## 题目来源

Seerc2009

