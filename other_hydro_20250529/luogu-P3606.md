## 题目描述
Farmer John is building a brand new, $N$-story barn, with the help of his $K$ cows ($1 \leq N \leq K \leq 10^{12}$ and $N \leq 10^5$). To build it as quickly as possible, he needs your help to figure out how to allocate work among the cows.

Each cow must be assigned to work on exactly one specific floor out of the $N$ total floors in the barn, and each floor must have at least one cow assigned to it. The $i$th floor requires $a_i$ units of total work, and each cow completes one unit of work per hour, so if $c$ cows work on floor $i$, it will be completed in $a_i / c$ units of time. For safety reasons, floor $i$ must be completed before construction can begin on floor $i+1$.

Please compute the minimum total time in which the barn can be completed, if the cows are allocated to work on floors in an optimal fashion. Output this number rounded to the nearest integer; it is guaranteed that the solution will be more than 0.1 from the boundary between two integers.

## 输入格式
The first line of input contains $N$ and $K$.

The next $N$ lines contain $a_1 \ldots a_N$, each a positive integer of size at most $10^{12}$.

## 输出格式
Please output the minimum time required to build the barn, rounded to the

nearest integer.



## 题目大意
### 题目大意
FJ 正在他的 $K$ 头奶牛的帮助下建造一个全新的 $N$ 层谷仓（$1\le N\le K\le 10^{12}，N\le 10^5$)。为了能够尽快的建造它，他需要你帮助他来找出如何在奶牛间分配工作。

每一头牛必须分配到 $N$ 层中的某一个特定楼层中，并且每一层楼必须至少有一头牛在其中工作。第i层楼需要 $a_i$ 个单位的工作，并且每一头牛完成每一单位的工作需要一个单位时间。所以如果有 $C$ 头牛在第 $i$ 层工作，那么第 $i$ 层需要 $\frac{a_i}{c}$ 个单位时间。为了安全起见，在开始施工第 $i+1$ 层楼之前，必须先完成第 $i$ 层。

如果奶牛被分配以最佳方式在楼层上工作，请计算完成谷仓的最小总时间。输出这个时间四舍五入到整数的结果；数据保证答案离两个整数间的中界大于 $0.1$。
### 输入格式
第一行包括两个数 $N$ 和 $K$。

接下来 $N$ 行包括了$a_1\dots a_n$，每行一个不大于 $10^{12}$ 的正整数。
### 输出格式
请输出完成谷仓的最小总时间（四舍五入至整数）。

by @Happy_mouse

```input1
2 5
10
4
```

```output1
5
```

