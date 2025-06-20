## 题目描述
Let's call the median of an array of length $(2 \cdot k + 1)$ the number that appears in position $(k + 1)$ after sorting its elements in non-decreasing order. For example, the medians of the arrays $[1]$, $[4,2,5]$, and $[6,5,1,2,3]$ are $1$, $4$, and $3$, respectively.

You are given an array of integers $a$ of **even** length $n$.

Determine whether it is possible to split $a$ into several subarrays of **odd** length such that all the medians of these subarrays are pairwise equal.

Formally, you need to determine whether there exists a sequence of integers $i_1, i_2, \ldots, i_k$ such that the following conditions are satisfied:

- $1 = i_1 < i_2 < \ldots < i_k = (n + 1)$;
- $(i_2 - i_1) \bmod 2 = (i_3 - i_2) \bmod 2 = \ldots = (i_k - i_{k - 1}) \bmod 2 = 1$;
- $f(a[i_1..(i_2-1)]) = f(a[i_2..(i_3-1)]) = \ldots = f(a[i_{k - 1}..(i_k - 1)])$, where $a[l..r]$ denotes the subarray consisting of elements $a_l, a_{l + 1}, \ldots, a_r$, and $f(a)$ denotes the median of the array $a$.

## 输入格式
The first line contains a single even integer $n$ ($2 \le n \le 2 \cdot 10^5$) --- the length of the array.

The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1\le a_i\le 10^9)$ --- the elements of the array.

It is guaranteed that $n$ is even.

## 输出格式
Output $\tt{Yes}$ if it is possible to divide $a$ into several subarrays of odd length in such a way that all medians of these subarrays are pairwise equal, and $\tt{No}$ otherwise.

```input1
4
1 1 1 1
```

```output1
Yes
```

```input2
6
1 2 3 3 2 1
```

```output2
Yes
```

```input3
6
1 2 1 3 2 3
```

```output3
No
```

## 提示
In the first example, the array $[1,1,1,1]$ can be divided into the arrays $[1]$ and $[1,1,1]$ with medians equal to $1$.

In the second example, the array $[1,2,3,3,2,1]$ can be divided into the arrays $[1,2,3]$ and $[3,2,1]$ with medians equal to $2$.

In the third example, the array $[1,2,1,3,2,3]$ cannot be divided into several arrays of odd length with the same median values.

### Scoring

- ($3$ points): $n=2$;
- ($14$ points): $1 \le a_i \le 2$ for $1\le i\le n$;
- ($12$ points): $a_i \le a_{i+1}$ for $1\le i < n$;
- ($16$ points): $1 \le a_i \le 3$ for $1 \le i \le n$; each value occurs in $a$ no more than $n \over 2$ times;
- ($17$ points): $n \le 100$;
- ($18$ points): $n \le 2000$;
- ($20$ points): no additional restrictions.

