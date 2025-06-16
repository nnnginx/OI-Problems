## 题目描述
You are given a set of $n$ points with integer coordinates. Each point has its own weight.

We can split the plane using a point of coordinates $(x, y)$ into four dials by drawing the vertical line in $x + 0.5$ and the horizontal line in $y + 0.5$. We define the weight of a dial to be the sum of the weights of all the points in that dial. Furthermore, the $\underline{\text{imbalance}}$ of such a split is the maximum difference between the weight of two of its dials.

For each integer $x$ such that $1 \leq x < n$, find the minimum imbalance of a split that uses a point on the vertical line $x$.

## 输入格式
The first line contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$).

Each of the next $n$ lines contains three integers $x_i$, $y_i$, and $w_i$ ($1 \leq x_i, y_i \leq n$, $1 \leq w_i \leq 10^9$) --- the coordinates and weight of the $i$-th point.

## 输出格式
The only line of the output should contain $n - 1$ integers, the required minimum imbalances.

```input1
4
3 2 5
4 4 2
1 4 4
2 2 1
```

```output1
6
4
6
```

## 提示
- ($7$ points): $1 \leq n \leq 200$;
- ($17$ points): $1 \leq n \leq 5000$;
- ($53$ points): $1 \leq n \leq 100\,000$;
- ($23$ points): no further restrictions.

