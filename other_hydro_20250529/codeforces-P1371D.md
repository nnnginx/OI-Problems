## Description

<div><p>A mad scientist Dr.Jubal has made a competitive programming task. Try to solve it!</p><p>You are given integers $n,k$. Construct a grid $A$ with size $n \times n$ <span class="tex-font-style-bf">consisting of integers $0$ and $1$</span>. The very important condition should be satisfied: the sum of all elements in the grid is exactly $k$. In other words, the number of $1$ in the grid is equal to $k$.</p><p>Let's define:</p><ul> <li> $A_{i,j}$ as the integer in the $i$-th row and the $j$-th column. </li><li> $R_i = A_{i,1}+A_{i,2}+...+A_{i,n}$ (for all $1 \le i \le n$). </li><li> $C_j = A_{1,j}+A_{2,j}+...+A_{n,j}$ (for all $1 \le j \le n$). </li><li> In other words, $R_i$ are row sums and $C_j$ are column sums of the grid $A$. </li><li> For the grid $A$ let's define the value $f(A) = (\max(R)-\min(R))^2 + (\max(C)-\min(C))^2$ (here for an integer sequence $X$ we define $\max(X)$ as the maximum value in $X$ and $\min(X)$ as the minimum value in $X$). </li></ul><p>Find any grid $A$, which satisfies the following condition. Among such grids find any, for which the value $f(A)$ is the minimum possible. Among such tables, you can find any.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;�� the number of test cases. Next $t$ lines contain descriptions of test cases.</p><p>For each test case the only line contains two integers $n$, $k$ $(1 \le n \le 300, 0 \le k \le n^2)$.</p><p>It is guaranteed that the sum of $n^2$ for all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, firstly print the minimum possible value of $f(A)$ among all tables, for which the condition is satisfied.</p><p>After that, print $n$ lines contain $n$ characters each. The $j$-th character in the $i$-th line should be equal to $A_{i,j}$.</p><p>If there are multiple answers you can print any.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;�� the number of test cases. Next $t$ lines contain descriptions of test cases.</p><p>For each test case the only line contains two integers $n$, $k$ $(1 \le n \le 300, 0 \le k \le n^2)$.</p><p>It is guaranteed that the sum of $n^2$ for all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, firstly print the minimum possible value of $f(A)$ among all tables, for which the condition is satisfied.</p><p>After that, print $n$ lines contain $n$ characters each. The $j$-th character in the $i$-th line should be equal to $A_{i,j}$.</p><p>If there are multiple answers you can print any.</p>

## Samples

```input1
4
2 2
3 8
1 0
4 16
```

```output1
0
10
01
2
111
111
101
0
0
0
1111
1111
1111
1111
```




## Note

<p>In the first test case, the sum of all elements in the grid is equal to $2$, so the condition is satisfied. $R_1 = 1, R_2 = 1$ and $C_1 = 1, C_2 = 1$. Then, $f(A) = (1-1)^2 + (1-1)^2 = 0$, which is the minimum possible value of $f(A)$.</p><p>In the second test case, the sum of all elements in the grid is equal to $8$, so the condition is satisfied. $R_1 = 3, R_2 = 3, R_3 = 2$ and $C_1 = 3, C_2 = 2, C_3 = 3$. Then, $f(A) = (3-2)^2 + (3-2)^2 = 2$. It can be proven, that it is the minimum possible value of $f(A)$.</p>
