## Description

<div><p>Monocarp is wandering through a matrix consisting of $2$ rows and $n$ columns. Let's denote the cell in the $i$-th row and $j$-th column as $(i, j)$. Monocarp starts at cell $(1, 1)$ and wants to reach cell $(2, n)$.</p><p>In one move, Monocarp can move in one of two directions: </p><ul> <li> right&nbsp;！ from cell $(i, j)$ to cell $(i, j + 1)$; </li><li> down&nbsp;！ from cell $(i, j)$ to cell $(i + 1, j)$. </li></ul><p>Monocarp can't go outside the matrix.</p><p>Polycarp wants to prevent Monocarp from freely wandering through the matrix. To do this, he wants to choose exactly $k$ different cells in the matrix and block them. He cannot choose cells $(1, 1)$ and $(2, n)$.</p><p>For each $i$ from $0$ to $n$, Polycarp wants to know how many ways he can block exactly $k$ cells, so that Monocarp has exactly $i$ different paths from $(1, 1)$ to $(2, n)$. Two paths are considered different if there exists a cell that Monocarp visits in one path but not in the other.</p><p>As the number of ways can be quite large, output it modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The only line contains two integers $n$ and $k$ ($2 \le n \le 2 \cdot 10^5$; $2 \le k \le 2 \cdot n - 2$)&nbsp;！ the number of columns in the matrix and the number of cells Polycarp wants to block.</p></div><div class="output-specification"><p>Output $n + 1$ integers: for each $i$ from $0$ to $n$, the number of ways to block exactly $k$ cells, so that Monocarp has exactly $i$ different paths from $(1, 1)$ to $(2, n)$. Output all answers modulo $10^9 + 7$.</p></div>

## Input

<p>The only line contains two integers $n$ and $k$ ($2 \le n \le 2 \cdot 10^5$; $2 \le k \le 2 \cdot n - 2$)&nbsp;！ the number of columns in the matrix and the number of cells Polycarp wants to block.</p>

## Output

<p>Output $n + 1$ integers: for each $i$ from $0$ to $n$, the number of ways to block exactly $k$ cells, so that Monocarp has exactly $i$ different paths from $(1, 1)$ to $(2, n)$. Output all answers modulo $10^9 + 7$.</p>





```input1|
2 2
```




```input2|
10 2
```




```input3|
10 5
```




```input4|
22 10
```




```output1
1 0 0
```




```output2
45 24 21 18 15 12 9 6 3 0 0
```




```output3
7812 420 210 90 30 6 0 0 0 0 0
```




```output4
467563090 1847560 1016158 534820 267410 125840 55055 22022 7865 2420 605 110 11 0 0 0 0 0 0 0 0 0 0
```


