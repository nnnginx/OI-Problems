## 题目描述
Bessie the cow was excited to recently return to in-person learning! Unfortunately, her instructor, Farmer John, is a very boring lecturer, and so she ends up falling asleep in class often.
Farmer John has noticed that Bessie has not been paying attention in class. He has asked another student in class, Elsie, to keep track of the number of times Bessie falls asleep in a given class. There are $N$ class periods $(1\le N\le 10^5)$, and Elsie logs that Bessie fell asleep $a_i$ times $(0\le a_i\le 10^6)$ in the $i$-th class period. The total number of times Bessie fell asleep across all class periods is at most $10^6$.

Elsie, feeling very competitive with Bessie, wants to make Farmer John feel like Bessie is consistently falling asleep the same number of times in every class -- making it appear that the issue is entirely Bessie's fault, with no dependence on Farmer John's sometimes-boring lectures. The only way Elsie may modify the log is by combining two adjacent class periods. For example, if $a=[1,2,3,4,5]$, then if Elsie combines the second and third class periods the log will become $[1,5,4,5]$.

Help Elsie compute the minimum number of modifications to the log that she needs to make so that she can make all the numbers in the log equal.

## 输入格式
Each input will contain $T$ $(1\le T\le 10)$ test cases that should be solved independently.

The first line contains $T$, the number of test cases to be solved. The $T$ test cases follow, each described by a pair of lines. The first line of each pair contains $N$, and the second contains $a_1,a_2,\ldots,a_N$. 

It is guaranteed that within each test case, the sum of all values in $a$ is at most $10^6$. It is also guaranteed that the sum of $N$ over all test cases is at most $10^5$.

## 输出格式
Please write $T$ lines of output, giving the minimum number of modifications Elsie could perform to make all the log entries equal for each case.

## 题目大意
### 题目描述

奶牛 Bessie 最近很高兴能够重返线下课堂！不幸的是，她的老师 Farmer John 讲课非常无聊，因此她经常在课堂上睡着。  
Farmer John 注意到 Bessie 在课堂上没有专心听讲。他让班上的另一位学生 Elsie 记录 Bessie 在每节课上睡着的次数。总共有 $N$ 节课（$1 \leq N \leq 10^5$），Elsie 记录到 Bessie 在第 $i$ 节课上睡着了 $a_i$ 次（$0 \leq a_i \leq 10^6$）。所有课程中 Bessie 睡着的总次数不超过 $10^6$。

Elsie 对 Bessie 感到非常竞争，她希望让 Farmer John 觉得 Bessie 在每节课上睡着的次数是一致的——让问题看起来完全是 Bessie 的错，而与 Farmer John 有时无聊的讲课无关。Elsie 修改记录的唯一方式是将两节相邻的课合并。例如，如果 $a = [1,2,3,4,5]$，那么如果 Elsie 合并第二和第三节课，记录将变为 $[1,5,4,5]$。

请帮助 Elsie 计算她需要对记录进行的最少修改次数，以使记录中的所有数字相等。

### 输入格式

每个输入包含 $T$（$1 \leq T \leq 10$）个需要独立解决的测试用例。

第一行包含 $T$，表示测试用例的数量。接下来的 $T$ 组测试用例，每组由两行描述。每组的第一行包含 $N$，第二行包含 $a_1, a_2, \ldots, a_N$。

保证每个测试用例中，$a$ 的所有值之和不超过 $10^6$。同时，所有测试用例的 $N$ 之和不超过 $10^5$。

### 输出格式

请输出 $T$ 行，每行表示 Elsie 为使记录中的所有数字相等所需的最少修改次数。

### 提示

对于第一个测试用例，Elsie 可以通过 3 次修改将记录改为全为 $3$：
```
   1 2 3 1 1 1
-> 3 3 1 1 1
-> 3 3 2 1
-> 3 3 3
```

对于第二个测试用例，Elsie 可以通过 2 次修改将记录改为全为 $7$：
```
   2 2 3
-> 2 5
-> 7
```

对于最后一个测试用例，Elsie 不需要进行任何操作，因为记录已经由相同的数字组成。

```input1
3
6
1 2 3 1 1 1
3
2 2 3
5
0 0 0 0 0
```

```output1
3
2
0
```

## 提示
【样例解释】

For the first test case in this example, Elsie can change her log to consist solely of 3s with 3 modifications.
```
   1 2 3 1 1 1
-> 3 3 1 1 1
-> 3 3 2 1
-> 3 3 3
```
For the second test case, Elsie can change her log to 7 with 2 modifications.
```
   2 2 3
-> 2 5
-> 7
```
For the last test case, Elsie doesn’t need to perform any operations; the log already consists of equal entries.

