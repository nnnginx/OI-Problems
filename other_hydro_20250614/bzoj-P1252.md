## 题目描述

A fuel station has infinite amount of each of $N$ kinds of fuel. Each kind of fuel has density $a_{i}$, cost $b_{i}$ and intensity $c_{i}$.$m$ kilograms of such fuel has volume $ma_{i}$, intensity $mc_{i}$ and costs $mb_{i}$ dollars. Your car can store any mixture of different kinds of fuel such that the overall volume does not exceed $A$. You have $B$ dollars. Your task is to determine the maximal overall intensity of the fuel you can buy. Note that you can buy any nonnegative amount of any kind of fuel, not necessarily an integer number of kilograms.

## 输入格式

The first line of the input contains three integers $N,A,B$ $(1 \leq N \leq 100000,1 \leq A,B  \leq 1000)$.Each of the next $N$ lines describes one kind of fuel. $i+1-st$ line contains three integers $a_{i},b_{i},c_{i} \ (a_i,b_i,c_i \leq 1000)$.

```input1
2 3 3
1 2 1
2 1 1
```

```output1
2.000
```

## 数据范围

对于所有的数据：

$0 \leq A,B \leq 10^5$

$0<a_i,b_i,c_i \leq 1000$

对于 $50\%$ 的数据：

$N \leq 100$

对于 $100\%$ 的数据：

$N \leq 10^5$

