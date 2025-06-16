# AT_code_festival_china_a Lock

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-festival-2014-china-open/tasks/code_festival_china_a

## 输入格式

Input is given in the following format.

> $ n $

- On the first line, you will be given $ n\ (1\ \leq\ n\ \leq\ 5) $, the number of digits of the dial lock.

## 输出格式

On the first line, output $ m $, the minimum number of procedures to try all combinations of digits.

On the following $ m+1 $ lines, output the combination of digits that appears during the trial in order. If there are more than $ 1 $ possible answer, you may choose any one of them. Make sure to insert a line break at the end of the last line.

## 输入输出样例 #1

### 输入 #1

```
1
```

### 输出 #1

```
9
0
1
2
3
4
5
6
7
8
9
```

## 输入输出样例 #2

### 输入 #2

```
2
```

### 输出 #2

```
99
00
01
02
03
04
05
06
07
08
09
19
18
17
16
15
14
13
12
11
10
20
21
22
23
24
25
26
27
28
29
39
38
37
36
35
34
33
32
31
30
40
41
42
43
44
45
46
47
48
49
59
58
57
56
55
54
53
52
51
50
60
61
62
63
64
65
66
67
68
69
79
78
77
76
75
74
73
72
71
70
80
81
82
83
84
85
86
87
88
89
99
98
97
96
95
94
93
92
91
90
```

## 说明/提示

### Problem

Alice has a box locked with $ n $ digits dial lock. Each dial of the lock can be set to a digit from $ 0 $ to $ 9 $. Unfortunately, she forgot the passcode (of $ n $ digits). Now she will try all possible combinations of digits to unlock the key.

She can do one of the following procedure each time.

- Choose $ 1 $ dial and add $ 1 $ to that digit. (If the digit chosen was $ 9 $, it will be $ 0 $).
- Choose $ 1 $ dial and subtract $ 1 $ from that digit. (If the digit chosen was $ 0 $, it will be $ 9 $).

Curiously, she wants to try all combinations even if she found the correct passcode during the trials. But it is a hard work to try all the $ 10^n $ combinations. Help her by showing the way how to make the procedure less as possible.

Initially, the combination of digits of the lock is set to $ 00..0 $.

Calculate $ m $, the minimum number of procedures to try all combinations of digits, and show the $ m+1 $ combinations of digits after each procedures, including the initial combination $ 00..0 $. If there are more than one possible answer, you may choose any one of them.

Checking if the current combination of digits matches the passcode doesn't count as a procedure.

### Sample Explanation 1

Don't forget to output the minimum number of procedures $ 9 $ on the first line. On the following lines, note that you have to output $ m+1 $ lines including the initial combination $ 0 $.