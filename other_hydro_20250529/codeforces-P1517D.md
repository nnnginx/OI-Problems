## Description

<div><p>You are wandering in the explorer space of the 2050 Conference.</p><p>The explorer space can be viewed as an undirected weighted grid graph with size $n\times m$. The set of vertices is $\{(i, j)|1\le i\le n, 1\le j\le m\}$. Two vertices $(i_1,j_1)$ and $(i_2, j_2)$ are connected by an edge if and only if $|i_1-i_2|+|j_1-j_2|=1$.</p><p>At each step, you can walk to any vertex connected by an edge with your current vertex. On each edge, there are some number of exhibits. Since you already know all the exhibits, whenever you go through an edge containing $x$ exhibits, your <span class="tex-font-style-it">boredness</span> increases by $x$.</p><p>For each starting vertex $(i, j)$, please answer the following question: What is the minimum possible boredness if you walk from $(i, j)$ and go back to it after exactly $k$ steps?</p><p>You can use any edge for multiple times but the boredness on those edges are also counted for multiple times. At each step, you cannot stay on your current vertex. You also cannot change direction while going through an edge. Before going back to your starting vertex $(i, j)$ after $k$ steps, you can visit $(i, j)$ (or not) freely.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$ and $k$ ($2\leq n, m\leq 500, 1\leq k\leq 20$).</p><p>The $j$-th number ($1\le j \le m - 1$) in the $i$-th line of the following $n$ lines is the number of exibits on the edge between vertex $(i, j)$ and vertex $(i, j+1)$. </p><p>The $j$-th number ($1\le j\le m$) in the $i$-th line of the following $n-1$ lines is the number of exibits on the edge between vertex $(i, j)$ and vertex $(i+1, j)$. </p><p>The number of exhibits on each edge is an integer between $1$ and $10^6$.</p></div><div class="output-specification"><p>Output $n$ lines with $m$ numbers each. The $j$-th number in the $i$-th line, $answer_{ij}$, should be the minimum possible boredness if you walk from $(i, j)$ and go back to it after exactly $k$ steps.</p><p>If you cannot go back to vertex $(i, j)$ after exactly $k$ steps, $answer_{ij}$ should be $-1$. </p></div>

## Input

<p>The first line contains three integers $n$, $m$ and $k$ ($2\leq n, m\leq 500, 1\leq k\leq 20$).</p><p>The $j$-th number ($1\le j \le m - 1$) in the $i$-th line of the following $n$ lines is the number of exibits on the edge between vertex $(i, j)$ and vertex $(i, j+1)$. </p><p>The $j$-th number ($1\le j\le m$) in the $i$-th line of the following $n-1$ lines is the number of exibits on the edge between vertex $(i, j)$ and vertex $(i+1, j)$. </p><p>The number of exhibits on each edge is an integer between $1$ and $10^6$.</p>

## Output

<p>Output $n$ lines with $m$ numbers each. The $j$-th number in the $i$-th line, $answer_{ij}$, should be the minimum possible boredness if you walk from $(i, j)$ and go back to it after exactly $k$ steps.</p><p>If you cannot go back to vertex $(i, j)$ after exactly $k$ steps, $answer_{ij}$ should be $-1$. </p>

## Samples

```input1
3 3 10
1 1
1 1
1 1
1 1 1
1 1 1
```

```output1
10 10 10
10 10 10
10 10 10
```






```input2
2 2 4
1
3
4 2
```

```output2
4 4
10 6
```






```input3
2 2 3
1
2
3 4
```

```output3
-1 -1
-1 -1
```




## Note

<p>In the first example, the answer is always $10$ no matter how you walk.</p><p>In the second example, $answer_{21} = 10$, the path is $(2,1) \to (1,1) \to (1,2) \to (2,2) \to (2,1)$, the boredness is $4 + 1 + 2 + 3 = 10$.</p>
