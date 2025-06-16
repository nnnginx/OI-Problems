## Description

<div><p>You are given a matrix of size $n \times m$, where the rows are numbered from $1$ to $n$ from top to bottom, and the columns are numbered from $1$ to $m$ from left to right. The element at the intersection of the $i$-th row and the $j$-th column is denoted by $a_{ij}$.</p><p>Consider the algorithm for stabilizing matrix $a$:</p><ol><li> Find the cell $(i, j)$ such that its value is strictly greater than the values of all its neighboring cells. If there is no such cell, terminate the algorithm. If there are multiple such cells, choose the cell with the smallest value of $i$, and if there are still multiple cells, choose the one with the smallest value of $j$.</li><li> Set $a_{ij} = a_{ij} - 1$. </li><li> Go to step $1$. </li></ol><p>In this problem, cells $(a, b)$ and $(c, d)$ are considered neighbors if they share a common side, i.e., $|a - c| + |b - d| = 1$.</p><p>Your task is to output the matrix $a$ after the stabilization algorithm has been executed. It can be shown that this algorithm cannot run for an infinite number of iterations.</p></div><div class="input-specification"><p>Each test consists of multiple sets of input data. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of sets of input data. This is followed by their description.</p><p>The first line of each set of input data contains two integers $n$ and $m$ ($1 \leq n, m \leq 100, n \cdot m &gt; 1$)&nbsp;！ the number of rows and columns of matrix $a$. </p><p>The next $n$ lines describe the corresponding rows of the matrix. The $i$-th line contains $m$ integers $a_{i1}, a_{i2}, \ldots, a_{im}$ ($1 \leq a_{ij} \leq 10^9$).</p><p>It is guaranteed that the sum of $n \cdot m$ over all sets of input data does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each set of input data, output $n$ lines with $m$ numbers in each line&nbsp;！ the values of the cells of matrix $a$ after the stabilization algorithm.</p></div>

## Input

<p>Each test consists of multiple sets of input data. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of sets of input data. This is followed by their description.</p><p>The first line of each set of input data contains two integers $n$ and $m$ ($1 \leq n, m \leq 100, n \cdot m &gt; 1$)&nbsp;！ the number of rows and columns of matrix $a$. </p><p>The next $n$ lines describe the corresponding rows of the matrix. The $i$-th line contains $m$ integers $a_{i1}, a_{i2}, \ldots, a_{im}$ ($1 \leq a_{ij} \leq 10^9$).</p><p>It is guaranteed that the sum of $n \cdot m$ over all sets of input data does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each set of input data, output $n$ lines with $m$ numbers in each line&nbsp;！ the values of the cells of matrix $a$ after the stabilization algorithm.</p>





```input1|2,3,7,8,9,13,14,15,16,17,18
6
1 2
3 1
2 1
1
1
2 2
1 2
3 4
2 3
7 4 5
1 8 10
5 4
92 74 31 74
74 92 17 7
31 17 92 3
74 7 3 92
7 31 1 1
3 3
1000000000 1 1000000000
1 1000000000 1
1000000000 1 1000000000
```




```output1
1 1 
1 
1 
1 2 
3 3 
4 4 5 
1 8 8 
74 74 31 31 
74 74 17 7 
31 17 17 3 
31 7 3 3 
7 7 1 1 
1 1 1 
1 1 1 
1 1 1
```



## Note

<p>In the first set of input data, the algorithm will select the cell $(1, 1)$ twice in a row and then terminate. </p><center> <img class="tex-graphics" src="./34753/file/YfqhzGqS.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second set of input data, there is no cell whose value is strictly greater than the values of all neighboring cells.</p><p>In the third set of input data, the algorithm will select the cell $(2, 2)$ and then terminate. </p><center> <img class="tex-graphics" src="./34753/file/zfryuHt3.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the fourth set of input data, the algorithm will select the cell $(1, 1)$ three times and then the cell $(2, 3)$ twice.</p><center> <img class="tex-graphics" src="./34753/file/dfPCkPw6.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
