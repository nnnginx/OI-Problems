## 题目描述
JOI-kun has $N$ go stones. The stones are numbered from $1$ to $N$. The color of each stone is an integer between $1$ and $10^9$, inclusive. In the beginning, the color of Stone $i$ ($1 \le i \le N$) is $A_i$.

From now, JOI-kun will perform $N$ operations. He will put the stones on the table in a line. The operation $i$ ($1 \le i \le N$) will be performed as follows:

1. JOI-kun will put Stone $i$ on the immediate right of Stone $i - 1$. However, when $i = 1$, JOI-kun will put Stone 1 on the table.
2. If there is a stone among Stones $1,2,\cdots,i-1$ whose current color is the same as Stone $i$, let $j$ be the maximum index of such stones, and JOI-kun will paint all of Stones $j+1,j+2,\cdots,i-1$ with the color $A_i$.

In order to confirm whether the operations are correctly performed, JOI-kun wants to know in advance the colors of the stones after all the operations are performed.

Given information of the go stones, write a program which determines the colors of the stones after the $N$ operations are performed.

## 输入格式
Read the following data from the standard input.

> $N$  
> $A_1$  
> $A_2$  
> $\vdots$  
> $A_N$

## 输出格式
Write $N$ lines to the standard output. The $i$-th line ($1 \le i \le N$) should contain the color of Stone $i$ after the $N$ operations are performed.

## 题目大意
JOI 君有 $N$ 枚棋子，棋子从 $1$ 到 $N$ 编号。每个棋子的颜色是介于 $1$ 和 $10^9$ 之间的整数，包括 $1$ 和 $10^9$。一开始，第 $i$（$1 \le i \le N$）枚棋子的颜色是 $A_i$。

接下来，JOI 君将执行 $N$ 步操作。他将把棋子放在桌子上排成一行。第 $i$（$1 \le i \le N$）步操作如下：

1. JOI 君会将第 $i$ 枚棋子放在第 $i - 1$ 枚棋子的紧邻的右侧。 特别地，当 $i = 1$ 时，JOI 君会直接将第 1 枚棋子放在桌子上。
2. 如果前 $i-1$ 枚棋子中有至少一枚棋子当前的颜色与棋子 $i$ 相同，设 $j$ 为这些棋子的编号的最大值，那么 JOI 君会把第 $j+1,j+2,\cdots,i-1$ 枚棋子的颜色都涂成 $A_i$。

为了确认操作有没有正确完成，JOI 君想提前知道所有操作完成后棋子的颜色。

给定棋子的信息，编写一个程序，确定在执行 $N$ 次操作后每枚棋子的颜色。

```input1
6
1
2
1
2
3
2

```

```output1
1
1
1
2
2
2

```

```input2
10
1
1
2
2
1
2
2
1
1
2

```

```output2
1
1
1
1
1
1
1
1
1
2

```

## 提示
## Samples

### Sample 1

The operations are performed as in the following table.

![](https://cdn.luogu.com.cn/upload/image_hosting/0newqhzt.png)

Finally, the colors of Stones 1, 2, 3, 4, 5, 6 will be 1, 1, 1, 2, 2, 2, respectively.

This sample input satisfies the constraints of Subtasks 1, 3.

### Sample 2

This sample input satisfies the constraints of all the subtasks.

## Constraints

- $1 \le N \le 2\times 10^5$.
- $1 \le A_i \le 10^9$ ($1 \le i \le N$).
- Given values are all integers.

## Subtasks

1. (25 points) $N \le 2 000$.
2. (35 points) $A_i \le 2$ ($1 \le i \le N$).
3. (40 points) No additional constraints.

