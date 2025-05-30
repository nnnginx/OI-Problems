## 题目描述
Define the ''digit product'' $f(x)$ of a positive integer $x$ as the product of all its digits. For example, $f(1234) = 1 \times 2 \times 3 \times 4 = 24$, and $f(100) = 1 \times 0 \times 0 = 0$.

Given two integers $l$ and $r$, please calculate the following value:
$$(\prod_{i=l}^r f(i)) \mod (10^9+7)$$ 
In case that you don't know what $\prod$ represents, the above expression is the same as 
$$(f(l) \times f(l+1) \times \dots \times f(r)) \mod (10^9+7)$$


## 输入格式
There are multiple test cases. The first line of the input contains an integer $T$ (about $10^5$), indicating the number of test cases. For each test case:

The first and only line contains two integers $l$ and $r$ ($1 \le l \le r \le 10^9$), indicating the given two integers. The integers are given without leading zeros.


## 输出格式
For each test case output one line containing one integer indicating the answer.

## 题目大意
**【题目描述】**

定义正整数 $x$ 的 "数字乘积" $f(x)$ 为其所有数字的乘积。例如，$f(1234) = 1 \times 2 \times 3 \times 4 = 24$，$f(100) = 1 \times 0 \times 0 = 0$。

给定两个整数 $l$ 和 $r$，请计算以下值：
$$(\prod_{i=l}^r f(i)) \mod (10^9+7)$$ 
如果你不知道 $\prod$ 表示什么，上述表达式等同于 
$$(f(l) \times f(l+1) \times \dots \times f(r)) \mod (10^9+7)$$

**【输入格式】**

有多个测试用例。输入的第一行包含一个整数 $T$（大约 $10^5$），表示测试用例的数量。对于每个测试用例：

第一行且唯一一行包含两个整数 $l$ 和 $r$（$1 \le l \le r \le 10^9$），表示给定的两个整数。这些整数没有前导零。

**【输出格式】**

对于每个测试用例，输出一行，包含一个整数，表示答案。

**【样例解释】**

对于第一个样例测试用例，答案是 $9! \mod (10^9+7) = 362880$。

对于第二个样例测试用例，答案是 $(f(97) \times f(98) \times f(99)) \mod (10^9+7) = (9 \times 7 \times 9 \times 8 \times 9 \times 9) \mod (10^9+7) = 367416$。

翻译来自于：[ChatGPT](https://chatgpt.com/)。

```input1
2
1 9
97 99

```

```output1
362880
367416

```

## 提示
For the first sample test case, the answer is $9! \mod (10^9+7) = 362880$.

For the second sample test case, the answer is $(f(97) \times f(98) \times f(99)) \mod (10^9+7) = (9 \times 7 \times 9 \times 8 \times 9 \times 9) \mod (10^9+7) = 367416$.


