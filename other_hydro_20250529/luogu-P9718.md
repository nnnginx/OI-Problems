## 题目描述
Given a positive integer $x$, find the minimum positive integer $y$ such that the number of $\textbf{carries}^1$ of $x+y$ is exactly $k$.

We adds numbers $\textbf{by column addition in base-ten}$, just like what we normally do in primary school. For example, there are two carries in the following addition.

![](https://cdn.luogu.com.cn/upload/image_hosting/pfnper3r.png)

$^1$ which means ``进位`` in Chinese.

## 输入格式
The first line contains an integer $T$ $(1\leq T\leq 10^5)$ $-$ the number of test cases.

For each test case, the first line contains two integers $x, k$ $(1\leq x < 10^{18}, 0\leq k \leq 18)$.

## 输出格式
For each test case, output one integer representing the answer in one line. If there is no solution, output $-1$ instead.

## 题目大意
**【题目描述】**

给定一个正整数 $x$，找到最小的正整数 $y$，使得 $x+y$ 的 $\textbf{进位}$ 数量恰好为 $k$。

我们按照十进制中的列加法进行相加，就像我们在小学时所做的那样。例如，下面的加法中有两次进位。

![](https://cdn.luogu.com.cn/upload/image_hosting/pfnper3r.png)

**【输入格式】**

第一行包含一个整数 $T$ $(1\leq T\leq 10^5)$ $-$ 测试用例的数量。

对于每个测试用例，第一行包含两个整数 $x, k$ $(1\leq x < 10^{18}, 0\leq k \leq 18)$。

**【输出格式】**

对于每个测试用例，输出一行一个整数，表示答案。如果没有解决方案，则输出 $-1$。

翻译来自于：[ChatGPT](https://chatgpt.com/)。

```input1
4
12345678 0
12345678 5
12345678 18
990099 5
```

```output1
1
54322
999999999987654322
9910
```

