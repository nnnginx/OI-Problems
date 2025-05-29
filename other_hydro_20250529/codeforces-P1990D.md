## Description

<div><p>You are given an array $a$ of size $n$.</p><p>There is an $n \times n$ grid. In the $i$-th row, the first $a_i$ cells are black and the other cells are white. In other words, note $(i,j)$ as the cell in the $i$-th row and $j$-th column, cells $(i,1), (i,2), \ldots, (i,a_i)$ are black, and cells $(i,a_i+1), \ldots, (i,n)$ are white.</p><p>You can do the following operations any number of times in any order: </p><ul> <li> Dye a $2 \times 2$ subgrid white; </li><li> Dye a whole row white. Note you can <span class="tex-font-style-bf">not</span> dye a whole column white. </li></ul><p>Find the minimum number of operations to dye all cells white.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>For each test case: </p><ul> <li> The first line contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;！ the size of the array $a$. </li><li> The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq n$). </li></ul><p>It's guaranteed that the sum of $n$ over all test cases will not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum number of operations to dye all cells white.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>For each test case: </p><ul> <li> The first line contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;！ the size of the array $a$. </li><li> The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq n$). </li></ul><p>It's guaranteed that the sum of $n$ over all test cases will not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum number of operations to dye all cells white.</p>





```input1|2,3,6,7,10,11,14,15,18,19
10
1
0
4
2 4 4 2
4
3 2 1 0
3
0 3 0
3
0 1 3
3
3 1 0
4
3 1 0 3
4
0 2 2 2
6
1 3 4 2 0 4
8
2 2 5 2 3 4 2 4
```




```output1
0
3
2
1
2
2
3
2
4
6
```



## Note

<p>In the first test case, you don't need to do any operation.</p><p>In the second test case, you can do:</p><ul> <li> Dye $(1,1), (1,2), (2,1)$, and $(2,2)$ white; </li><li> Dye $(2,3), (2,4), (3,3)$, and $(3,4)$ white; </li><li> Dye $(3,1), (3,2), (4,1)$, and $(4,2)$ white. </li></ul><p>It can be proven $3$ is the minimum number of operations.</p><p>In the third test case, you can do:</p><ul> <li> Dye the first row white; </li><li> Dye $(2,1), (2,2), (3,1)$, and $(3,2)$ white. </li></ul><p>It can be proven $2$ is the minimum number of operations.</p>
