## 题目描述
A prefix sum array of an integer array $a$ of length $n$ is an array $b$ of length $n$ such that $b_i = a_1+a_2+\ldots+a_i$.

A suffix sum array of an integer array $a$ of length $n$ is an array $b$ of length $n$ such that $b_i = a_n+a_{n-1}+\ldots+a_i$.

We call the **normalization** of an integer array $a$ of length $n$ performing the assignment $a_i \leftarrow \max(\min(a_i, 10^{18}),-10^{18})$ for $1 \le i \le n$.

An integer array $a$ of length $n$ is given.

We are allowed to perform operations of three types:

- replace each element of array $a$ with its opposite (perform the assignment $a_i \leftarrow (-a_i)$ for $1 \le i \le n$);
- select any subsegment of the array $a$ and replace it with the array of its prefix sums, then **normalize** array $a$;
- select any subsegment of the array $a$ and replace it with the array of its suffix sums, then **normalize** array $a$.

Find the shortest sequence of operations required to make all elements of array $a$ non-negative.

Note that for some blocks of tests, it is allowed to find a sequence of operations that is not the shortest possible.

## 输入格式
The first line contains two integers $n$ and $g$ ($1 \le n \le 2 \cdot 10^5$, $0 \le g \le 8$) --- the length of the array and the test group number, respectively.

The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($-1 \le a_i \le 1$) --- the elements of the array.

## 输出格式
In the first line, print a single integer $m$~--- the minimum number of operations required to make all elements of the array $a$ non-negative.

In the next $m$ lines, output the descriptions of the operations. Output the descriptions of operations of the first type in the format "$\texttt{1}$". Output the descriptions of operations of the second and third types in the formats "$\texttt{2 l r}$" and "$\texttt{3 l r}$", respectively, where $l$ and $r$ ($1 \le l \le r \le n$) denote the left and right boundaries of the subarray of the corresponding operation.

If there are multiple correct answers, any of them may be printed.

```input1
7 0
0 0 1 -1 -1 -1 1
```

```output1
2
3 1 3
2 1 7
```

## 提示
In the first example, the array $a$ changes twice:
- after performing the third type of operation with parameters $l=1$, $r=3$, the array $a$ becomes equal to $[1,1,1,-1,-1,-1,1]$;
- after performing the second type of operation with parameters $l=1$, $r=7$, the array $a$ becomes equal to $[1,2,3,2,1,0,1]$.

### Scoring

Let the minimum number of operations required to make all elements of the array $a$ non-negative for a certain test be $m_{ans}$, and your solution uses $m_{user}$ operations.

- ($14$ points): $m_{ans} \le 1$;
- ($17$ points): your solution will be considered correct if $m_{user} \le 100$. It can be proved that there always exists a sequence of no more than $100$ operations under the given constraints;
- ($18$ points): your solution will be considered correct if $m_{user} \le m_{ans} + 3$;
- ($7$ points): your solution will be considered correct if $m_{user} \le m_{ans} + 1$;
- ($7$ points): $n \le 3000$; it is guaranteed that **all** shortest sequences of operations contain **only** operations of the second type;
- ($19$ points): it is guaranteed that **all** shortest sequences of operations contain **only** operations of the second type;
- ($17$ points): $n \le 3000$;
- ($1$ point): no additional constraints.

