## 题目描述
Given an array of integers $a$ of length $n$.

You can modify the array using the **addition operation**. To apply the **addition operation**, you need to perform three sequential actions:

- Choose any integer $x$.
- Choose any subarray $[l;r]$ of the array.
- Add $x$ to each element of the chosen subarray (perform the assignment operation $a_i \leftarrow (a_i+x)$ for $l \le i\le r$).

Find the minimum number of **addition operations** required to make all elements of the array $a$ pairwise distinct.

## 输入格式
The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) --- the length of the array.

The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le 10^9$) --- the elements of the array.

## 输出格式
Output a single integer --- the minimum number of **addition operations** required to make all elements of the array $a$ pairwise distinct.

```input1
3
1 2 3
```

```output1
0
```

```input2
5
2 3 2 3 2
```

```output2
2
```

```input3
9
2 3 1 1 3 2 1 3 3
```

```output3
2
```

## 提示
In the first example, all elements of the array $a$ are pairwise distinct.

In the second example, after applying two \textit{addition operations} with parameters $x=-3$, $l=1$, $r=2$ and $x=-1$, $l=1$, $r=3$, the array $a$ becomes equal to $[-2,-1,1,3,2]$.

In the third example, after applying two \textit{addition operations} with parameters $x=-3$, $l=4$, $r=8$ and $x=-10$, $l=7$, $r=9$, the array $a$ becomes equal to $[2,3,1,-2,0,-1,-12,-10,-7]$.

### Scoring

- ($9$ points): all elements of the array $a$ are equal to $1$.
- ($15$ points): $1 \le a_i \le 2$ for $1 \le i \le n$; $a_i \le a_{i+1}$ for $1 \le i < n$.
- ($14$ points): $n \le 8$.
- ($17$ points): $a_1 = a_n$.
- ($12$ points): $n \le 2000$.
- ($12$ points): $1 \le a_i \le 100$ for $1\le i\le n$.
- ($21$ points): no additional constraints.

