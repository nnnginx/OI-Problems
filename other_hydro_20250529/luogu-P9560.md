## 题目描述
Given two positive integers $n$ and $k$, you can perform the following two types of operations any number of times (including zero times):

- Choose an integer $x$ which satisfies $0 \leq x < k$, and change $n$ into $k\cdot n+x$. It will cost you $a$ coins to perform this operation once. The integer $x$ you choose each time can be different.
- Change $n$ into $\lfloor \frac{n}{k} \rfloor$. It will cost you $b$ coins to perform this operation once. Note that $\lfloor \frac{n}{k} \rfloor$ is the largest integer which is less than or equal to $\frac{n}{k}$.

Given a positive integer $m$, calculate the minimum number of coins needed to change $n$ into a multiple of $m$. Please note that $0$ is a multiple of any positive integer.


## 输入格式
There are multiple test cases. The first line of the input contains an integer $T$ ($1\leq T\leq 10^5$) indicating the number of test cases. For each test case:

The first line contains five integers $n$, $k$, $m$, $a$, $b$ ($1\leq n\leq 10^{18}$, $1\leq k, m, a, b\leq 10^9$).

## 输出格式
For each test case output one line containing one integer, indicating the minimum number of coins needed to change $n$ into a multiple of $m$. If this goal cannot be achieved, output $-1$ instead.

## 题目大意
**【题目描述】**

给定两个正整数 $n$ 和 $k$，您可以进行以下两种操作任意次（包括零次）：

- 选择一个整数 $x$ 满足 $0 \leq x < k$，将 $n$ 变为 $k\cdot n+x$。该操作每次花费 $a$ 枚金币。每次选择的整数 $x$ 可以不同。
- 将 $n$ 变为 $\lfloor \frac{n}{k} \rfloor$。该操作每次花费 $b$ 枚金币。其中 $\lfloor \frac{n}{k} \rfloor$ 表示小于等于 $\frac{n}{k}$ 的最大整数。

给定正整数 $m$，求将 $n$ 变为 $m$ 的倍数最少需要花费几枚金币。请注意：$0$ 是任何正整数的倍数。

**【输入格式】**

有多组测试数据。第一行输入一个整数 $T$（$1\leq T\leq 10^5$）表示测试数据组数。对于每组测试数据：

第一行输入五个正整数 $n$，$k$，$m$，$a$，$b$（$1\leq n\leq 10^{18}$，$1\leq k, m, a, b\leq 10^9$）。

**【输出格式】**

每组数据输出一行一个整数，代表将 $n$ 变为 $m$ 的倍数最少需要花费几枚金币。如果无法完成该目标，输出 $-1$。

**【样例解释】**

对于第一组样例数据，一开始 $n=101$，最优操作如下：

- 首先进行一次第二种操作，将 $n$ 变为 $\lfloor \frac{n}{4} \rfloor=25$，花费 $5$ 枚金币。
- 接下来进行一次第一种操作，选择 $x = 3$，将 $n$ 变为 $4\cdot n+3=103$，花费 $3$ 枚金币。
- 接下来进行一次第一种操作，选择 $x = 2$，将 $n$ 变为 $4\cdot n+2=414$，花费 $3$ 枚金币。
- 此时 $414=2 \times 207$，满足 $n$ 是 $m$ 的倍数。共花费 $5+3+3=11$ 枚金币。

对于第二组样例数据，进行两次第二种操作将 $n$ 变为 $0$。共花费 $1 + 1 = 2$ 枚金币。

对于第三组样例数据，因为 $n = 114 = 6 \times 19$ 已经是 $m$ 的倍数，因此无需进行任何操作。共花费 $0$ 枚金币。

```input1
4
101 4 207 3 5
8 3 16 100 1
114 514 19 19 810
1 1 3 1 1
```

```output1
11
2
0
-1
```

## 提示
For the first sample test case, initially $n=101$. The optimal steps are shown as follows:

- Firstly, perform the second type of operation once. Change $n$ into $\lfloor \frac{n}{4} \rfloor=25$. This step costs $5$ coins.
- Then, perform the first type of operation once. Choose $x = 3$ and change $n$ into $4\cdot n+3=103$. This step costs $3$ coins.
- Then, perform the first type of operation once. Choose $x = 2$ and change $n$ into $4\cdot n+2=414$. This step costs $3$ coins.
- As $414=2 \times 207$, $n$ is a multiple of $m$. The total cost is $5+3+3=11$ coins.

For the second sample test case, perform the second type of operation twice will change $n$ into $0$. The total cost is $1 + 1 = 2$ coins.

For the third sample test case, as $n = 114 = 6 \times 19$ is already a multiple of $m$, no operation is needed. The total cost is $0$ coins.

