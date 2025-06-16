## 题目描述
To qualify for cow camp, Bessie needs to earn a good score on the last problem of the USACOW Open contest. This problem has $T$ distinct test cases $(2≤T≤10^3)$ weighted equally, with the first test case being the sample case. Her final score will equal the number of test cases that her last submission passes.
Unfortunately, Bessie is way too tired to think about the problem, but since the answer to each test case is either "yes" or "no," she has a plan! Precisely, she decides to repeatedly submit the following nondeterministic solution:
```
if input == sample_input:
  print sample_output
else:
  print "yes" or "no" each with probability 1/2, independently for each test case
```
Note that for all test cases besides the sample, this program may produce a different output when resubmitted, so the number of test cases that it passes will vary.

Bessie knows that she cannot submit more than $K$ $(1≤K≤10^9)$ times in total because then she will certainly be disqualified. What is the maximum possible expected value of Bessie's final score, assuming that she follows the optimal strategy?

## 输入格式
The only line of input contains two space-separated integers $T$ and $K$.

## 输出格式
The answer as a decimal that differs by at most $10^{−6}$ absolute or relative error from the actual answer.

## 题目大意
### 题目描述

为了获得参加奶牛训练营的资格，Bessie 需要在 USACOW 公开赛的最后一题中取得好成绩。这道题有 $T$ 个独立的测试用例（$2 \leq T \leq 10^3$），权重相同，其中第一个测试用例是样例。她的最终得分将等于她最后一次提交通过的测试用例数量。

不幸的是，Bessie 太累了，无法思考这个问题，但由于每个测试用例的答案要么是“yes”，要么是“no”，她想到了一个计划！具体来说，她决定反复提交以下非确定性解决方案：

```
if input == sample_input:
    print sample_output
else:
    print "yes" or "no" each with probability 1/2, independently for each test case
```

注意，对于除样例之外的所有测试用例，这个程序在重新提交时可能会产生不同的输出，因此它通过的测试用例数量会有所不同。

Bessie 知道她总共不能提交超过 $K$ 次（$1 \leq K \leq 10^9$），否则她肯定会被取消资格。假设 Bessie 遵循最优策略，她的最终得分的最大可能期望值是多少？

### 输入格式

输入只有一行，包含两个用空格分隔的整数 $T$ 和 $K$。

### 输出格式

输出一个十进制数，表示答案，与实际答案的绝对误差或相对误差不超过 $10^{-6}$。

### 样例解释 1

在这个例子中，Bessie 应该继续重新提交，直到她提交了 3 次或获得了满分。Bessie 获得满分的概率是 $\frac{7}{8}$，获得一半分数的概率是 $\frac{1}{8}$，因此在这种策略下，Bessie 的最终得分的期望值是 $\frac{7}{8} \cdot 2 + \frac{1}{8} \cdot 1 = \frac{15}{8} = 1.875$。从这个公式可以看出，Bessie 得分的期望值可以通过对所有可能的得分 $x$ 求和 $p(x) \cdot x$ 来计算，其中 $p(x)$ 是获得得分 $x$ 的概率。

### 样例解释 2

在这里，Bessie 应该只在第一次尝试通过少于 3 个测试用例时才提交第二次。

### 数据范围

- 测试用例 3-6 满足 $T \leq 25$ 且 $K \leq 100$。
- 测试用例 7-9 满足 $K \leq 10^6$。
- 测试用例 10-17 没有额外限制。

```input1
2 3
```

```output1
1.875
```

```input2
4 2
```

```output2
2.8750000000000000000
```

## 提示
【样例解释 1】

In this example, Bessie should keep resubmitting until she has reached 3 submissions or she receives full credit. Bessie will receive full credit with probability $\frac 78$ and half credit with probability $\frac 18$, so the expected value of Bessie's final score under this strategy is $\frac 78\cdot 2+\frac 18\cdot 1=\frac {15}{8}=1.875$. As we see from this formula, the expected value of Bessie's score can be calculated by taking the sum over $x$ of $p(x)\cdot x$, where $p(x)$ is the probability of receiving a score of $x$.

【样例解释 2】

Here, Bessie should only submit twice if she passes fewer than 3 test cases on her first try.

【数据范围】

- Test cases 3-6 satisfy $T≤25$ and $K≤100$.
- Test cases 7-9 satisfy $K≤10^6$.
- Test cases 10-17 satisfy no additional constraints.

