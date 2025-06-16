## 题目背景
译自 CCC 2025 Senior T2。本题满分为 $15$。

## 题目描述
给定一个小写字母组成的字符串 $s$ 和一个非负整数 $c$。你需要求出，将这个字符串无限重复后，第 $c$ 个位置上的字符是什么。注意字符串是 $\text{0}-\text{indexed}$ 的，也就是 $s_0$ 是第一个字符。

为了减少输入量，我们将字符串做了压缩：具体地，我们将一段连续的相同字母 $\underbrace{\texttt{aa}\cdots\texttt{aa}}_{k\text{ 个}}$ 压缩成字母+出现次数 $\texttt{a}k$ 的形式。例如，$\texttt{aaaabccdddd}$ 被压缩成 $\texttt{a4b1c2d4}$。


## 输入格式
第一行，一个只含小写字母和数字的压缩后的字符串 $s'$。

第二行，一个非负整数 $c$。

## 输出格式
一个小写字母，表示答案。

```input1
r2d2
8
```

```output1
r
```

```input2
a4b1c2d10
100
```

```output2
d
```

## 提示

#### 样例解释

- 样例 $1$ 解释：$\texttt{r2d2}$ 压缩前是 $\texttt{rrdd}$。

重复无数多次即为 $\texttt{rrddrrdd\textcolor{red}{r}rdd}\cdots$。

- 样例 $2$ 解释：$\texttt{a4b1c2d10}$ 压缩前是 $\texttt{aaaabccdddddddddd}$。




#### 子任务

对于 $100\%$ 的数据，保证：

- $2\le |s'|\le 10^5$；
- $s'$ 中出现的整数的范围是 $[1,10^{12}]$；
- $0\le c\le 10^{12}$。

---

- $\text{Subtask 0(0 points})$：样例。
- $\text{Subtask 1(6 points})$：
	- $0\le c\le 2\times 10^3$；
	- $s'$ 中出现的整数的范围是 $[1,9]$；
    - 压缩前，$s$ 的长度不超过 $2000$。
- $\text{Subtask 2(3 points})$：
	- $0\le c\le 10^6$；
    - 压缩前，$s$ 的长度不超过 $10^6$。
- $\text{Subtask 3(3 points})$：
    - 压缩前，$s$ 的长度不超过 $10^6$。
- $\text{Subtask 4(3 points})$：无特殊限制。

