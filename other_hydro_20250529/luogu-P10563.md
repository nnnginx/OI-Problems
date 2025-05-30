## 题目描述
There is a two-dimensional plane.
    
    
    
You have a set of points $\{(x_i,y_i)\}$ that satisfies $1\le x_i\le n, 1\le y_i\le m$ (Both $x_i$ and $y_i$ are integers), and there are no two points with the same coordinates.
    
    
    
If two points have the same horizontal or vertical coordinates, we will connect an edge between these two points. This forms a graph.
    
    
    
You need to find the sum of the maximum number of matches in the graphs formed by all possible $2^{nm}-1$ non empty sets, and output the result modulo $998244353$.
    
    
    
Here, the maximum number of matches in a graph is defined as: selecting the most edges so that there are no common vertices between any two edges.

## 输入格式

There are multiple testcases in this problem.
    
    
    
The first line contains an integer $T(1\le T\le 100)$, which represents the number of testcases.
    
    
    
Each of the testcases contains two integers $n,m(1\leq n,m\leq 500)$.

## 输出格式
 
For each of the testcases, print an integer representing the result modulo $998244353$.
    

```input1
10
1 1
1 2
2 2
4 4
3 3
5 5
1 8
20 20
100 100
500 500
```

```output1
0
1
10
241456
964
200419152
448
985051144
370696900
357517517
```

