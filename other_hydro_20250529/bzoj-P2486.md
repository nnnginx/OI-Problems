## 题目描述

I have a set of super poker cards，consisting of an infinite number of cards．For each positive integer $p$，there are exactly four cards whose value is $p$：Spade（$S$），Heart（$H$），Club（$C$） and Diamond（$D$）．There are no cards of other values．  
Given two positive integers $n$ and $k$，how many ways can you pick up at most $k$ cards whose values sum to $n$？For example，if $n=15$ and $k=3$，ne way is $3H+4S+8H$，shown below：  
![](./2036/file/pic1.jpg)

## 输入格式

There will be at most $20$ test cases，each with two integers $n$ and $k$．The input is terminated by $n=k=0$．

## 输出格式

For each test case，print the number of ways，modulo $1 \times 10^9 +9$．

```input1
2 1
2 2
2 3
50 5
0 0
```

```output1
4
10
10
1823966
```

## 数据规模与约定

$100\%$ 的数据满足：$1 \le n,k \le 10$。

## 提示

湖南省第七届大学生程序设计大赛

## 题目来源

鸣谢刘汝佳先生授权使用


