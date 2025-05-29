## 题目描述

有 $n$ 个阵地，已知我方在每个阵地上的士兵数，若我方士兵不为 $0$ 则表示该阵地由我方占领，否则为对方占领。某些阵地之间有通道，我们认为士兵可以经过 $1$ 单位时间从 $1$ 个阵地移动到相邻（有通道相连）的阵地。对于一个阵地，如果其相邻的阵地中有非我方阵地，则表示其受到威胁，该阵地中我方人数。   
现在求：对我方士兵进行一次 $1$ 个单位的移动（调动），在保证我方不丢失阵地的情况下（即我方每个阵地上的人数不为 $0$），使得我方所有受到威胁的阵地中人数最少的阵地的人数尽可能多。

## 输入格式

On the first line a positive integer: the number of test cases, at most 100. After that per test case: 
One line with an integer $n$: the number of regions.   
One line with $n$ integers $a_{i}$: the number of your armies on each region. A number 0 indicates that a region is controlled by your opponents, while a positive number indicates that it is under your control.   
$n$ lines with $n$ characters, where each character is either `Y` or `N`. The $i$-th character of the $j$-th line is `Y` if regions $i$ and $j$ border, and `N` otherwise. This relationship is symmetric and the $i$-th character of the $i$-th line will always be `N`. 
In every test case, you control at least one region, and your opponents control at least one region. Furthermore, at least one of your regions borders at least one of your opponents' regions. 

## 输出格式

Per test case: 
One line with an integer: the maximum number of armies on your weakest border region after one turn of moving.

```input1
2 
3 
1 1 0 
NYN 
YNY 
NYN 
7 
7 3 3 2 0 0 5 
NYNNNNN 
YNYYNNN 
NYNYYNN 
NYYNYNN 
NNYYNNN 
NNNNNNY 
NNNNNYN

```

```output1
1
4
```

## 数据规模与约定

对于 $100\%$ 的数据，满足 $1 \leq n \leq  100$，$0 \leq a_{i} \leq 100$，$1 \leq \text{数据组数} \leq 100$。

## 题目来源

Nwerc2010


