## 题目描述
给出 $N$ 件单位时间任务，对于第 $i$ 件任务，如果要完成该任务，需要占用 $[S_i,T_i]$ 间的某个时刻，且完成后会有 $V_i$ 的收益。一个时刻只能做一件任务，做一个任务也只需要一个时刻。求最大收益。

## 输入格式
第一行一个整数 $N$，表示可供选择的任务个数。接下来的第二到第 $N+1$ 行，每行三个数，其中第 $i+1$ 行依次为 $Si,Ti,Vi$。

## 输出格式

输出最大收益。

## 样例输入
```plain
4
1 1 2
2 2 2
1 2 3
1 3 1
```
## 样例输出
```plain
6
```
## 样例解释
共有四个任务，其中第一个任务只能在时刻 $1$ 完成，第二个任务只能在时刻 $2$ 做，第三个任务只能在时刻 $1$ 或时刻 $2$ 做，第四个任务可以在 $[1,3]$ 内任一时刻完成，四个任务的价值分别为 $2$、$2$、$3$ 和 $1$。一种完成方案是：时刻 $1$ 完成第一个任务，时刻 $2$ 完成第三个任务，时刻 $3$ 完成第四个任务，这样得到的总收益为 $2+3+1=6$，为最大值。

## 数据规模与约定
对于 $100\%$ 的数据，$N \leq 5\times10^3$，$1 \leq S_i \leq T_i, V_i \leq 10^8$。

## 题目来源
版权所有者：冯齐纬