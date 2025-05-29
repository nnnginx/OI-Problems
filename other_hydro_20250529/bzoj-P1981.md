## 题目描述

We are looking into building a very long fence. We have already found a nice place to build it, and all that remains is to collect the materials. From local hardware stores, we can buy unlimited numbers of wooden boards, each of which can come in a variety of different lengths. To avoid waste, we want to make sure that the total length of these boards is exactly equal to the length of the fence we are trying to build. Given the length of the fence, and the possible board lengths that we can use, what is the minimum number of boards that we need to purchase in order to get exactly the right length? Beware: the fence is going to be very long!

## 输入格式

The first line of the input file contains the number of cases, $T$. $T$ test cases follow. Each test case consists of two lines.

The first line contains space-separated integers $l$ and $n$. These represent the total length of the fence, and the number of different board lengths that can be purchased.

The second line contains $n$ space-separated integers $b_1, b_2, \ldots, b_n$, representing all the possible board lengths.

## 输出格式

For each test case, output one line containing `Case #x: M`, where $x$ is the case number (starting from 1) and $M$ is as follows:

- If it is possible to purchase one or more boards so that their total length is exactly equal to $l$, then $M$ should be the minimum number of boards required to do this.
- Otherwise, $M$ should be the string `IMPOSSIBLE`.


```input1
2
10000000001 3
23 51 100
10000000001 3
100 52 22
```

```output1
Case #1: 100000004
Case #2: IMPOSSIBLE
```

## 样例说明 1

In the first example, the optimal strategy is to use $2$ boards of length $23$, $5$ boards of length $51$, and $99999997$ boards of length $100$. Of course, you could use just $100000001$ boards of length $100$ to get a total greater than $l$, but that is not allowed.

In the second example, it is only possible to get even lengths.

## 数据规模与约定

For all the test cases, limits $1 \le T \le 50$, $10^{10} \le l \le 10^{18}$, $1 \le n \le 100$.

All the $b_i$ values in a single test case are distinct. Small dataset $1 \le b_i \le 100$. Large dataset $1 \le b_i \le 10^5$.

## 题目来源

鸣谢成都七中 Zxytim。

Round 3。