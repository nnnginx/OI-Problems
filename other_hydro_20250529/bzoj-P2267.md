## 题目描述

Telephone Network

A telephone company wants to build a new telephone network in a city．The company has the goal that each person in the city should be able to call each other person．Of course，it is not possible to build direct connections between every pair of persons．Instead，the company uses a network made up of several layers．

We denote a network switch in layer $j$ by $S_j$．A switch $S_0$ consists of one input，one output and a cable connecting the input to the output．A switch $S_j$ with $j > 0$ consists of $2^j$ inputs，$2^j$ outputs and two switches $S^{j−1}$．

Input $i$ of $S_j$（$0 \le i < 2^j$） is connected via a cable to the inputs $i \mod 2^{j−1}$ of each of the two switches $S_{j−1}$．Similarly，output $i$ of $S_j$ is connected to the outputs $i \mod 2^{j−1}$ of each of the two switches $S_{j−1}$．

一个电话公司想在城市中搭建一个电话网络，他们的目标是让每两个人之间都能够通话。当然，在每两个用户之间直接搭一根电话线是不大可能的事情。于是公司采用了分层网络来解决这个问题。我们令第 $j$ 层网络由开关 $S_j$ 来控制。开关 $S_0$ 包含一个输入，一个输出和一条将输入和输出连起来的电话线。开关 $S_j$（$j > 0$） 包含 $2^j$ 个输入，$2^j$ 个输出和两个 $S_{j-1}$ 级的开关。$S_j$ 的第 $i$ 个输入是用线连接到 $S_{j-1}$ 的 $i \mod 2^{j−1}$ 上。同样，输出也是这么连接的。

![](./1817/file/pic1.png)

We are considering a network with one switch $S_n$ in the outermost layer．It can be shown that any input and output of switch $S_n$ has a unique connection path to any of the $S_0$ switches．Therefore，any input of $S_n$ can be connected to any of its outputs，and the connection path is uniquely determined by specifying through which switch $S_0$ the connection is established．

We number the switches $S_0$ belonging to the switch $S_n$ from $0$ to $2^n−1$．The $i$-th switch $S_0$ is defined as follows．Write the number $i$ in binary as $b_{n−1},b_{n−2} \dots b_0$．This defines a path from an input of $S_n$ to the $i$-th switch $S_0$ via the following procedure：for each $j$ ，$b_j ＝ 0$ indicates that the path extends from $S_{j+1}$ to the first $S_j$ switch to which it is directly connected，and $b_j ＝ 1$ indicates that the path extends to the second $S_j$ switch. Note that regardless of which input of $S_n$ is selected，this path arrives at the same $S_0$ switch，which is given the number $i$．See also the figure below the sample data for details of how the numbering works．

Sometimes multiple connections are needed at the same time．In order to avoid interference，each of the inputs and outputs of all switches $S_j$（$0 \le j \le n$） can be used by at most one connection．Given a set of connection requests，can you find connection paths for each request such that the connection paths are disjoint？

最外层网络只有一个开关 $S_n$。对已知 $S_n$ 的任意一个输入和输出，他们都有一条独特的路径连接到 $S_0$。因此，任意一个输入和输出就能够连接起来，而且这样的路径是独一无二的有连接到 $S_0$ 的路径决定的。我们将 $S_n$ 的 $2^n$ 个 $S_0$ 级开关标号为 $0$～$2^n−1$。第$i$ 个开关的定义为：将 $i$ 写成二进制 $b_{n−1},b_{n−2} \dots b_0$。$S_n$ 到 $S_0$ 的路径是这么确定的：对于每一位 $j$，$b_j ＝ 0$ 就表示 $S_{j+1}$ 连接到第一个 $S_j$ 开关，否则连接到第二个 $S_j$ 开关。对于给定的 $i$ ，无论开关 $S_n$ 的输入是什么，这个路径必须到达同一个 $S_0$ 开关。不懂的就好好看样例。有时候多组连接必须同时使用，为了防止交叉干扰，每个开关只能在这些通话中使用一次。给你一些通话需求，你能找到满足所有要求且不相交的路径么？

## 输入格式

**本题有多组数据**

On the first line a positive integer：the number of test cases，at most $100$．After that per test case：

One line with two integers $n$ and $m$：the layer of the outermost switch and the number of connection requests．

$m$ lines，each with two integers $a_i$ and $b_i$．Each such line represents a connection request from input number $a_i$ of $S_n$ to output number $b_i$．You may assume that the integers $a_i$ are pairwise distinct，and the integers $b_i$ are pairwise distinct as well．

**第一行一个正整数，表示测试数据，最多** $100$ **组.**

**然后每一组包括：**

**第一个两个数** $n,m$ **：网络的层数和连接需求数。**

**接下来** $m$ **行，每行包括两个正整数** $a_i$ **和** $b_i$**。表示输入和输出的编号。**$a_i$ **和** $b_i$ **只会出现一次。**

## 输出格式

Per test case：
One line with $m$ integers $s_1，\dots ，s_m$，where $s_i$ is the number of the $S_0$ switch through which the connection of input $a_i$ to output $b_i$ is established．

The connection paths should be disjoint．You may print any valid solution，and you may assume that there is at least one valid solution．

**Per test case：**

$m$ **个正整数** $s_1,\dots ,s_m$，$s_i$ **是** $a_i$ **到** $b_i$ **的连接路径**

**连接必须不相交。输出任意一个合法路径，并且路径是存在的。** 

```input1
2
1 1
0 1
3 5
0 3
1 4
2 5
3 6
4 7
```

```output1
0
3 0 1 2 4
```

## 样例解释 1 

3 5 ---　$3$ 层网络，$5$ 个连接

0 3

1 4

2 5

3 6

4 7

输入就这样了

输出

第一个 $3$

二进制表示为 $011$

表示 $0$ 先连最外层的第一个开关，下一层是第二个，在下层第二个。这样就连接到最底层

图上每一个圈都有两条线

选 $0$ 时就是上面一条，选 $1$ 就是下面一条

![](./1817/file/pic2.png)

## 题目来源

鸣谢南航 勇敢的加菲猫

## 数据规模与约定

$100\%$ 的数据满足：$1 \le n \le 16$，$1 \le m \le 2^n$，$0 \le a_i,b_i ＜ 2^n$。

