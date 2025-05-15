# 题目描述

众所周知，$\texttt{Alice}$ 和 $\texttt{Bob}$ 是一对好朋友。今天，他们约好一起玩游戏。

一开始，他们各自有一张空白的纸条。接下来，他们会在纸条上依次写 $n$ 个 $[1，m]$ 范围内的正整数。等 $\texttt{Alice}$ 写完，$\texttt{Bob}$ 在看到 $\texttt{Alice}$ 写的纸条之后开始写他的纸条。

$\texttt{Alice}$ 需要保证她写下的第 $i$ 个数在集合 $\mathrm{S}_{i}$ 中，$\texttt{Bob}$ 需要保证他写下的第 $i$ 个数在集合 $\mathrm{T}_{i}$ 中。题目保证 $1 \leq\left|\mathrm{S}_{i}\right|,\left|\mathrm{T}_{i}\right| \leq 2$ 。

$\texttt{Alice}$ 喜欢相同，因此，她希望她写下的数与 $\texttt{Bob}$ 写下的数对应位置相同的个数尽 量多。$\texttt{Bob}$ 喜欢不同，因此，他希望他写下的 $n$ 个数 $b_{1}, \cdots，b_{n}$ 互不相同。在此基础上，$\texttt{Bob}$ 希望他写下的数与 $\texttt{Alice}$ 写下的数对应位置相同的个数尽量少。

即设 $\texttt{Alice}$ 写下的数为 $a_{1}, \cdots，a_{n}$，$\texttt{Bob}$ 写下的数为 $b_{1}, \cdots，b_{n}$，记 $X$ 为满足 $1 \leq$ $i \leq n，a_{i}=b_{i}$ 的下标 $i$ 的个数，则

- $\texttt{Alice}$ 希望最大化 $X$。
- $\texttt{Bob}$ 在保证 $b_{1}, \cdots，b_{n}$ 互不相同的前提希望最小化 $X$。

你首先想知道 $\texttt{Bob}$ 能否保证他写下的 $n$ 个数互不相同。如果 $\texttt{Bob}$ 能够做到，你想 知道在双方均采取最优策略的前提下 $X$ 的值会是多少。

# 输入格式

本题有多组测试数据。

输入的第一行包含一个正整数 $T$，表示测试数据组数。

接下来包含 $T$ 组数据，每组数据的格式如下：

第一行包含两个正整数 $n，m$，表示纸条上需要写的数的个数和数的值域。

接下来 $n$ 行，每行输入的第一个整数为 $\left|\mathrm{S}_{i}\right|$ 表示集合 $\mathrm{S}_{i}$ 的元素个数，接下来输入$\left|\mathrm{S}_{i}\right|$ 个正整数描述 $\mathrm{S}_{i}$ 中的元素。

接下来 $n$ 行，每行输入的第一个整数为 $\left|\mathrm{T}_{i}\right|$ 表示集合 $\mathrm{T}_{i}$ 的元素个数，接下来输入
$\left|\mathrm{T}_{i}\right|$ 个正整数描述 $\mathrm{T}_{i}$ 中的元素。

# 输出格式

对于每组测试数据输出一行：若 $\texttt{Bob}$ 无法做到他写下的 $n$ 个数互不相同，输出 -1 ;

否则输出在双方均予取最优策略的前提下 $X$ 的值。

# 样例 #1

### 样例输入 #1

```
1
3 4
1 3
2 1 2
2 3 4
2 1 2
2 2 3
2 3 4
```

### 样例输出 #1

```
1
```

# 提示

## 样例解释

【样例 1 解释】

在这组样例中，$\mathrm{S}_{1}=\{3\}, \mathrm{S}_{2}=\mathrm{T}_{1}=\{1,2\}, \mathrm{S}_{3}=\mathrm{T}_{3}=\{3,4\}, \mathrm{T}_{2}=\{2,3\}$ 。

$\texttt{Alice}$ 的填法有 4 种，列举如下:

第一种: $a_{1}=3，a_{2}=1，a_{3}=3$ 。

第二种: $a_{1}=3，a_{2}=1，a_{3}=4$ 。

第三种: $a_{1}=3，a_{2}=2，a_{3}=3$ 。

第四种: $a_{1}=3，a_{2}=2，a_{3}=4$ 。

由于 $\texttt{Bob}$ 必须保证他所填的数互不相同，所以他有以下填法:

第一种: $b_{1}=1，b_{2}=2，b_{3}=3$ 。

第二种: $b_{1}=2，b_{3}=3，b_{3}=4$ 。

第三种: $b_{1}=1，b_{2}=2，b_{3}=4$ 。

第四种: $b_{1}=1，b_{2}=3，b_{3}=4$ 。

若 $\texttt{Alice}$ 选择第一种填法，则 $\texttt{Bob}$ 为最小化 $X$，选择第二种填法，得到 $X=0$ 。

若 $\texttt{Alice}$ 选择第三种填法，则 $\texttt{Bob}$ 为最小化 $X$，选择第一种填法，得到 $X=0$ 。

若 $\texttt{Alice}$ 选择第四种填法，则 $\texttt{Bob}$ 无论选择哪种填法，$X$ 均不小于 1。

因此，$\texttt{Alice}$ 为最大化 $X$ 的值，她会选择第四种填法。

表格中 $\sum n，\sum m$ 分别表示同个测试点内所有测试数据的 $n$ 总和和 $m$ 总和。$\sum n^{2}, \sum m^{2}, \sum n^{3}, \sum m^{3}$ 的含义类似。

![](https://cdn.luogu.com.cn/upload/image_hosting/m7eydvw8.png)

特殊性质 $\texttt{A}$：对于任何 $1\le i\le n$，$\mathrm{S}_i$ 和 $\mathrm{T}_i$ 互不相交，即 $\mathrm{S}_i ∩ \mathrm{T}_i=\empty$。

特殊性质 $\texttt{B}$：$n \geq 3$，且对于任侏何 $1 \le i < n，\mathrm{T}_{i}=\{i,i+1\}$，且 $\mathrm{T}_{n}=\{n,1\}$ 。

特殊性质 $\texttt{C}$：对于任何 $1 \leq i \leq n,\left|\mathrm{S}_{i}\right|=1$。

特殊性质 $\texttt{D}$：对于任何 $1 \leq i \leq n，\mathrm{S}_{i}=\mathrm{T}_{i}$。

## IO 提示

本题部分测试点输入规模较大，我们建议你采取效率较高的读入方式。

