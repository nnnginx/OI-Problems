## 题目描述
Farmer John is arranging his $N$ cows in a line to take a photo ($1 \leq N \leq 50$). The height of the $i$th cow in sequence is $a(i)$, and Farmer John thinks it would make for an aesthetically pleasing photo if the cow lineup has a large increasing subsequence of cows by height.

To recall, a subsequence is a subset $a(i_1), a(i_2), \ldots, a(i_k)$ of elements from the cow sequence, found at some series of indices $i_1 < i_2 < \ldots < i_k$. We say the subsequence is increasing if $a(i_1) \leq a(i_2) \leq \ldots \leq a(i_k)$.

FJ would like there to be a long increasing subsequence within his ordering of the cows. In order to ensure this, he allows himself initially to choose any subsequence and reverse its elements.

For example, if we had the list

```
1 6 2 3 4 3 5 3 4
```

We can reverse the chosen elements

```
1 6 2 3 4 3 5 3 4
  ^         ^ ^ ^
```
to get

```
1 4 2 3 4 3 3 5 6
  ^         ^ ^ ^
```
Observe how the subsequence being reversed ends up using the same indices as it initially occupied, leaving the other elements unchanged.

Please find the maximum possible length of an increasing subsequence, given that you can choose to reverse an arbitrary subsequence once.

## 输入格式
The first line of input contains $N$. The remaining $N$ lines contain $a(1) \ldots a(N)$, each an integer in the range $1 \ldots 50$.

## 输出格式
Output the number of elements that can possibly form a longest increasing subsequence after reversing the contents of at most one subsequence.

## 题目大意
### 题目描述

Farmer John 正在将他的 $N$ 头奶牛排成一列拍照（$1 \leq N \leq 50$）。序列中第 $i$ 头奶牛的高度为 $a(i)$，Farmer John 认为如果奶牛队列中存在一个较长的按高度递增的子序列，那么这张照片会更具美感。

回顾一下，子序列是指从奶牛序列中选出的一组元素 $a(i_1), a(i_2), \ldots, a(i_k)$，这些元素位于一系列索引 $i_1 < i_2 < \ldots < i_k$ 处。如果满足 $a(i_1) \leq a(i_2) \leq \ldots \leq a(i_k)$，则称该子序列是递增的。

FJ 希望在他的奶牛排列中存在一个较长的递增子序列。为了确保这一点，他允许自己最初选择任意一个子序列并将其元素反转。

例如，如果我们有以下序列：

```
1 6 2 3 4 3 5 3 4
```

我们可以反转选中的元素：

```
1 6 2 3 4 3 5 3 4
  ^         ^ ^ ^
```

得到：

```
1 4 2 3 4 3 3 5 6
  ^         ^ ^ ^
```

注意被反转的子序列最终仍然使用最初占据的索引，而其他元素保持不变。

请找出在最多反转一个子序列的情况下，可能的最长递增子序列的长度。

### 输入格式

输入的第一行包含 $N$。接下来的 $N$ 行包含 $a(1) \ldots a(N)$，每个数均为 $1$ 到 $50$ 之间的整数。

### 输出格式

输出在最多反转一个子序列后，可能形成的最长递增子序列的元素个数。

```input1
9
1
2
3
9
5
6
8
7
4
```

```output1
9

```

