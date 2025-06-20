# AT_bitflyer2018_final_b 交通費

## 题目描述

作为一次竞赛的组织者，你需要求出所有参与比赛的选手的交通费用，并支付该费用。参与比赛的选手共有 $n$ 人，他们都住在同一条道路上，而比赛场馆也设在这条道路上。已知第 $i$ 名选手的编号为 $i$，如果视道路为一条数轴，则他（她）家在这个数轴上表示数 $x_i$ 的点的位置。数据保证，对于满足 $1 \le i <n$ 的所有整数 $i$，一定有 $x_i<x_{i+1}$。

比赛场馆设在数轴上表示数 $c$ 的位置上。对于每位选手来说，他（她）的费用都有一个基准值 $d$。如果选手 $i$ 的家距离比赛场馆的距离（即 $|x_i-c|$）不大于 $d$ 个单位长度，则该选手的费用为 $|x_i-c|$ 元；否则，该选手的费用为 $d$ 元。

现在，你挑出了 $q$ 种比赛场馆的备选方案，其中，在第 $i$ 种方案中，比赛场馆的位置在数轴上表示 $c_i$ 的点上，费用的基准值为 $d_i$。现在，请按照 $i=1,2,...,q$ 的顺序回答：对于第 $i$ 种场馆选择方案，所有选手一共需要的费用为多少元？

## 输入格式

输入共 $(q+2)$ 行。第一行输入两个以单个空格隔开的正整数 $n$ 和 $q$，第二行输入 $n$ 名选手的家的位置 $x_1,x_2,...,x_n$，相邻的两个数之间以单个空格隔开。接下来的 $q$ 行中，按照 $i=1,2,...,q$ 的顺序输入第 $i$ 种方案所对应的场馆位置 $c_i$ 和基准值 $d_i$，中间以单个空格隔开。

## 输出格式

输出 $q$ 行。每行一个整数，即对应的场馆选择方案所需要的费用之和。

## 输入输出样例 #1

### 输入 #1

```
5 3
1 5 10 20 30
7 3
10 20
100 10
```

### 输出 #1

```
14
44
50
```

## 输入输出样例 #2

### 输入 #2

```
6 3
0 1 2 999999998 999999999 1000000000
0 0
100 99
1000000000 1000000000
```

### 输出 #2

```
0
593
3000000000
```

## 输入输出样例 #3

### 输入 #3

```
7 5
590 593 633 642 743 859 872
642 850108511
743 153
633 20
642 0
842 60895346
```

### 输出 #3

```
658
759
109
0
1056
```

## 说明/提示

**【输入输出样例 #1 解释】**

以第一组 $c,d$ 为例，每位选手所需要的费用金额依次为 $3,2,3,3,3$ 元，共计 $14$ 元，输出 $14$ 。

**数据规模与约定**

对于全部测试点，输入数据保证：

- $1 \le n,q \le 10^5$；
- $0 \le x_i,c_i,d_i \le 10^9$；
- 所有数值均为整数。