## 题目描述

Farmer John is constructing a new milking machine and wishes to keep it secret as long as possible. He has hidden in it deep within his farm and needs to be able to get to the machine without being detected. He must make a total of $t \ (1 \le  t \le  200)$ trips to the machine during its construction. He has a secret tunnel that he uses only for the return trips. The farm comprises $n \ (2 \le  n \le  200)$ landmarks (numbered $1\dots n$) connected by $p \ (1 \le  p \le  4\times 10^4)$ bidirectional trails (numbered $1\dots p$) and with a positive length that does not exceed $10^6$. Multiple trails might join a pair of landmarks. To minimize his chances of detection, FJ knows he cannot use any trail on the farm more than once and that he should try to use the shortest trails. Help FJ get from the barn (landmark $1$) to the secret milking machine (landmark $n$) a total of $t$ times. Find the minimum possible length of the longest single trail that he will have to use, subject to the constraint that he use no trail more than once.(Note well：The goal is to minimize the length of the longest trail, not the sum of the trail lengths.) It is guaranteed that FJ can make all $t$ trips without reusing a trail.

约翰正在制造一台新型的挤奶机，但他不希望别人知道。他希望尽可能久地隐藏这个秘密。他把挤奶机藏在他的农场里，使它不被发现。在挤奶机制造的过程中，他需要去挤奶机所在的地方 $t$ 次。他的农场里有秘密的地道，但约翰只在返回的时候用它。农场被划分成 $n$ 块区域，用 $1$ 到 $200$ 标号。这些区域被 $p$ 条道路连接，每条路有一个小于 $10^6$ 的长度 $l$。两块区域之间可能有多条道路连接。为了减少被发现的可能，约翰不会两次经过农场上的任何一条道路。当然了，他希望走最短的路。请帮助约翰寻找这 $t$ 次从仓库走到挤奶机所在地的路线。仓库是区域 $1$，挤奶机所在地是区域 $n$。我们现在要求的是约翰经过的这些道路中最长的路的长度最小是多少，当然他不能重复走某一条路。请注意，我们要求的不是最短的总路程长度，而是所经过的直揍连接两个区域的道路中最长的道路的最小长度。数据保证约翰可以找到 $t$ 条没有重复的从仓库到挤奶机所在区域的路。

## 输入格式

* Line $1$: Three space-separated integers: $n,p$, and $t$.
* Lines $2\dots p+1$: Line $i+1$ contains three space-separated integers,$a_i,b_i$, and $l_i$, indicating that a trail connects landmark $a_i$ to landmark $b_i$ with length $l_i$.
* 第 $1$ 行是 3 个整数 $n$、$p$ 和 $t$，用空格隔开。
* 第 $2$ 到 $p+1$ 行，每行包括 3 个整数，$a_i$，$b_i$，$l_i$。表示区域 $a_i$、$b_i$ 之间有一条长度为 $l_i$ 的道路。

## 输出格式

* Line $1$: A single integer that is the minimum possible length of the longest segment of Farmer John's route.
* 输出只有一行，包含一个整数，即约翰经过的这些道路中最长的路的最小长度。

```input1
7 9 2
1 2 2
2 3 5
3 7 5
1 4 1
4 3 1
4 5 7
5 7 1
1 6 3
6 7 3
```

```output1
5
```

## 样例说明

约翰选择 $1\to 2\to 3\to 7$ 和 $1\to 6\to 7$ 两条路线。这些路线中最长路的最小长度是 $5$。

## 数据规模与约定
对于 $100\%$ 的数据，$1 \leq t \leq 200$，$2 \leq n \leq 200$，$1 \leq p \leq 4\times 10^4$，$0\le l\le 10^6$。
## 题目来源

Gold