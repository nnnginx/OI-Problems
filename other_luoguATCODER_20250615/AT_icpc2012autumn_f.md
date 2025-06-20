# AT_icpc2012autumn_f Counting 1&#39;s

## 题目描述

设 $b_i(x)$ 是 $x$ 的第 $i$ 位最低有效位，即在二进制中 $(i \ge 1)$ 时 $x$ 的第 $i$ 位最低有效位。例如:
$6=(110)_2,b_1(6)=0,b_2(6)=1,b_3(6)=1,b_4(6)=0,b_5(6)=0$，等等。

设 $A$ 、$B$ 为满足 $1 \le A \le B \le 10^{18}$ 的整数，$k_i$ 为 $A \le x \le B$ 且 $b_i(x)=1$ 的整数个数。

你的任务是编写一个程序，为给定的 $\{ki\}$ 确定 $A$ 和 $B$。

## 输入格式

```
n
k_1
k_2
...
k_n
```
每个测试数据的第一行包含一个整数 $n(1 \le n \le64)$ 。然后有 $n$ 行，每一行包含
$k_i(0 \le k_i \le 2^{63}-1)$ 。对于所有 $i>n$ 的情况， $k_i=0$ 。
输入以 $n=0$ 结束，不需要对它进行输出。

## 输出格式

对于每个数据集，输出一行。
- 如果 $A$ 和 $B$ 可以只有一组，则输出 $A$ 和 $B$ ，两个数字之间用一个空格隔开。
- 如果存在的 $A$ 和 $B$多于一组 ，输出"Many"(不带引号)。
- 否则，如果不存在 $A$ 和 $B$ ，则输出"None"(不带引号)。

### 输入输出样例

输入样例
```
3
2
2
1
49
95351238128934
95351238128934
95351238128932
95351238128936
95351238128936
95351238128936
95351238128960
95351238128900
95351238128896
95351238129096
95351238128772
95351238129096
95351238129096
95351238126156
95351238131712
95351238131712
95351238149576
95351238093388
95351238084040
95351237962316
95351238295552
95351237911684
95351237911684
95351235149824
95351233717380
95351249496652
95351249496652
95351226761216
95351226761216
95351082722436
95351082722436
95352054803020
95352156464260
95348273971200
95348273971200
95354202286668
95356451431556
95356451431556
95346024826312
95356451431556
95356451431556
94557999988736
94256939803780
94256939803780
102741546035788
87649443431880
87649443431880
140737488355328
32684288648324
64
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
10
11
12
13
14
15
16
17
18
19
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
30
31
32
33
34
35
36
37
38
39
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
50
51
52
53
54
55
56
57
58
59
60
61
62
63
11
0
0
1
1
1
0
1
1
1
1
1
63
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
0
1
4
1
1
1
1
0
```
输出样例
```
1 4
123456789101112 314159265358979
None
2012 2012
None
Many
```