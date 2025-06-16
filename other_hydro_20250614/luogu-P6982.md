## 题目描述
Consider a toy interactive problem ONEMAX which is defined as follows.

You know an integer $n$ and there is a hidden bit - string $S$ of length $n$. The only thing you may do is to present the system a bit - string $Q$ of length $n$, and the system will return the number $\text{ONEMAX}(Q)$ — the number of bits which coincide in $Q$ and $S$ at the corresponding positions. The name of ONEMAX problem stems from the fact that this problem and a simpler one explaining when $S = 11\ldots11$, so that the problem turns into maximization (MAX) of the number of ones (ONE).

When $n$ is even, there is a similar (but harder) interactive problem called JUMP. The simplest way to describe the JUMP is by using ONEMAX:
$$
\text{JUMP}(Q)=
\begin{cases}
\text{ONEMAX}(Q) & \text{if } \text{ONEMAX}(Q)=n \text{ or } \text{ONEMAX}(Q)=n/2; \\
0 & \text{otherwise.}
\end{cases}
$$
Basically, the only nonzero values of ONEMAX which you can see with JUMP are $n$ (which means you've found the hidden string $S$) and $n/2$.

Given an even integer $n$ — the problem size, you have to solve the JUMP problem for the hidden string $S$ by making interactive JUMP queries. Your task is to eventually make a query $Q$ such that $Q = S$.

### Interaction protocol

First, the testing system tells the length of the bit - string $n$. Then, your solution asks the queries and the system answers them as given by the JUMP definition. When a solution asks the query $Q$ such that $Q = S$, the system answers $n$ and terminates, so if your solution, after reading the answer $n$, tries reading or writing anything, it will fail.

The limit on the number of queries is $n + 500$. If your solution asks a $(n + 501)$ - th query, then you will receive the “Wrong Answer” outcome. You will also receive this outcome if your solution terminates too early.

If your query contains wrong characters (neither 0, nor 1), or has a wrong length (not equal to $n$), the system will terminate the testing and you will receive the “Presentation Error” outcome.

You will receive the “Time Limit Exceeded” outcome and other errors for the usual violations.

Finally, if everything is OK (e.g. your solution finds the hidden string) on every test, you will receive the “Accepted” outcome, in this case you will have solved the problem.

## 输入格式
The first line of the input stream contains an even number $n$ ($2\leq n\leq1000$). The next lines of the input stream consist of the answers to the corresponding queries. Each answer is an integer — either $0$, $n/2$, or $n$. Each answer is on its own line.

## 输出格式
To make a query, print a line which contains a string of length $n$ which consists of characters $0$ and $1$ only. Don't forget to put a newline character and to flush the output stream after you print your query. 

## 题目大意
给定长度为 $n$（$n$ 为偶数） 的 01 字符串 $S$。

你可以向交互库进行询问。你可以向交互库输出一个长度为 $n$ 的 01 字符串 $Q$。设 $S$ 和 $Q$ 有 $k$ 个对应的位置上的字符相同。若 $k=n$ 或 $k=\frac n 2$，则交互库将返回 $k$，否则交互库将返回 $0$。

你最多向交互库询问 $n+500$ 次，要求求出 $S$。你只需要使最后一次询问的返回值为 $n$ 即可。此时你应立即结束程序，否则将得到不可预料的结果。

若你的字符串长度不为 $n$ 或出现 01 以外的字符，或者你的询问次数超过上限，则交互库会返回 $-1$。此时你应立即结束程序，否则将得到不可预料的结果。

$1\leq n\leq 1000$。

```input1
2
1
0
1
2
```

```output1
01
11
10
00
```

