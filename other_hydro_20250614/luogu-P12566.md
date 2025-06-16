## 题目描述
There are $k$ arrays of integers $a_1, a_2, \ldots, a_k$, where the array with index $i$ contains $l_i$ elements. Let $n = l_1 + l_2 + \ldots + l_k$.

You need to find $k$ integers $d_1, d_2, \ldots, d_k$ such that the numbers $(a_{i,j} + d_i)$ are pairwise distinct and satisfy $1 \leq a_{i,j} + d_i \leq n$.

## 输入格式
The first line contains two integers $n$ and $k$ ($1 \le n \le 10^4$, $1 \le k \le 5$) -- the total number of elements in the arrays and the number of arrays, respectively.

The next $k$ lines contain the arrays. The $i$-th line contains an integer $l_i$ ($1\le l_i\le n$) and $l_i$ integers $a_{i,1},a_{i,2},\ldots,a_{i,l_i}$ ($1 \le a_{i,j} \le n$) -- the length and elements of the $i$-th array, respectively.

It is guaranteed that $n = l_1 + l_2 + \ldots + l_k$.

## 输出格式
If the required values of $d$ do not exist, output a single line ``No``.

Otherwise, output ``Yes`` on the first line.

On the second line, output $k$ integers $d_1,d_2,\ldots,d_k$ -- the values that need to be added to the elements of the arrays to form a total of $n$ distinct integers from $1$ to $n$.

If there are multiple correct answers, any one of them may be output.

```input1
5 5
1 1
1 2
1 3
1 4
1 5
```

```output1
Yes
0 0 0 0 0
```

```input2
6 4
2 2 3
1 6
1 4
2 1 5
```

```output2
Yes
1 -5 1 1
```

```input3
7 2
4 1 4 5 6
3 1 2 6
```

```output3
Yes
0 1
```

```input4
4 2
2 2 3
2 2 4
```

```output4
No
```

## 提示
In the first example, $d = [0,0,0,0,0]$ satisfies the condition, since after adding the corresponding values, the arrays $[1]$, $[2]$, $[3]$, $[4]$, $[5]$ are formed.

In the second example, $d = [1,-5,1,1]$ satisfies the condition, since after adding the corresponding values, the arrays $[3,4]$, $[1]$, $[5]$, $[2,6]$ are formed.

In the third example, $d = [0,1]$ satisfies the condition, since after adding the corresponding values, the arrays $[1,4,5,6]$ and $[2,3,7]$ are formed.

### Scoring

- ($8$ points): $k=1$;
- ($9$ points): $a_{i,j}+1=a_{i,j+1}$ for $1 \le i \le k$, $1 \le j < l_i$;
- ($15$ points): $k \le 2$;
- ($21$ points): $k \le 3$;
- ($10$ points): $a_{i,j}+2=a_{i,j+1}$ for $1 \le i \le k$, $1 \le j < l_i$;
- ($10$ points): $(\max_{j \in [1;l_i]} a_{i,j}) - (\min_{j \in [1;l_i]} a_{i,j})=(n-k)$ for $1 \le i \le k$;
- ($10$ points): $n \le 30$;
- ($17$ points): without additional constraints.

