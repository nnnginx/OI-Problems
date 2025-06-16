## 题目描述
You are given a matrix of size $n \times m$ consisting of elements $a_{i,j}$. 

We call a **triangle** on the matrix of size $k$ starting at point $(x;y)$ a set of points that can be reached from $(x;y)$ in no more than $k$ steps going either up or right. 

You are asked to find for each $(x;y)$ $(k \le x \le n, 1 \le y \le m-k+1)$ the following values:

- The maximal value in the triangle of size $k$ starting at point $(x;y)$;
- The number of occurrences of the maximal value in that triangle.

## 输入格式
The first line contains three integers $n$, $m$, and $k$ $(1 \le n,m \le 2\,000, 1 \le k \le \min(n,m))$ --- dimensions of the matrix and the size of the triangle.

The following $n$ lines contain $m$ integers $a_{i,j}$ $(0 \le a_{i,j} \le 10^6)$ --- description of the matrix.

## 输出格式
Print two matrices of size $(n-k+1)\times(m-k+1)$. 

The first matrix in position $(i;j)$ should contain the maximal value of a triangle of size $k$ starting at $(i+k-1;j)$.

The second matrix in position $(i;j)$ should contain the number of occurrences of the maximal value in the triangle of size $k$ starting at $(i+k-1;j)$.

```input1
4 4 2
1 2 6 14
12 3 13 5
11 4 7 8
10 16 9 15
```

```output1
12 13 13 
12 7 13 
16 16 15 
1 1 1 
1 1 1 
1 1 1 
```

## 提示
- ($5$ points) $n,m \le 20$;
- ($10$ points) $n,m \le 100$;
- ($30$ points) $a_{i,j} \le 1$;
- ($35$ points) $n,m \le 1\,000$;
- ($20$ points) no additional restrictions.

