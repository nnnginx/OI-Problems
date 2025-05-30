UPD 15:22 来自出题人的提醒：注意题面里写的是非负整数，即 $n,m$ 可以为 $0$ ！

----------------------------------

## 题目描述

`Life` 有 $n$ 个边长为 $2$ 的大立方体和 $m$ 个边长为 $1$ 的小立方体。

现在 `Life` 想用一个长方体箱子把立方体们全部装箱，使得箱子的体积 $V$ 最小（可以自由指定箱子的长宽高，立方体允许悬空）。

但是这个问题对于 `Life` 而言太过困难，于是 `Life` 找到了你，你能帮他解决这个问题吗？

## 输入格式

**本题一组测试用例中包含多组数据**

第一行包含一个正整数 $T$，表示数据组数。

接下来 $T$ 行，每行包含两个**非负**整数，表示给定的 $n$ 和 $m$。

## 输出格式

共 $T$ 行，每行一个非负整数，表示所需的最小箱子体积 $V$。

## 样例输入 
```
3
1 19
1 546
732534654745769 457034535
```
## 样例输出 
```
27
555
5860277695000688
```

## 数据范围
**本题开启Subtask**

| 子任务编号 | $T<=$ | $n,m<=$ | 特殊性质 | 分值 | 依赖项 |
| :-: | :-: | :-: | :-: | :-: | :-: |
| $1$ | $10^2$ | $10^2$ | 无 | $10$ | 无 |
| $2$ | $10^2$ | $10^4$ | 无 | $10$ | 1 |
| $3$ | $10^3$ | $10^6$ | 无 | $10$ | 1,2 |
| $4$ | $2\times 10^2$ | $10^{14}$ | $m=4k,k\in \mathbb{N}$ | $5$ | 无 |
| $5$ | $2\times 10^2$ | $10^{14}$ | $m\leq 4$ | $10$ | 无 |
| $6$ | $10^3$ | $10^{10}$ | 无 | $20$ | 1,2,3 |
| $7$ | $4\times 10^2$ | $5\times 10^{11}$ | 无 | $15$ | 1,2,3,6 |
| $8$ | $2\times 10^2$ | $10^{14}$ | 无 | $20$ | 1,2,3,4,5,6,7 |